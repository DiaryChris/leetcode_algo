## Binary Search

2020.06.25

今天的目标，就是熟悉二分法的思路和写法。

二分法的思路很简单。小时候有个综艺节目，猜家电的价格，如果能够准确猜对，就把相应的家电送给参与者。譬如一台电视机价格为2000块。

我们第一次猜：3000。

主持人：高了。

那我们第二次肯定不会猜2999，否则要想猜到正确的价格，需要尝试1000次！

既然高了，我们又知道价格肯定在0-3000块之间。

第二次就折中猜一个：1500块。

主持人这回又说：低了。

现在我们就知道了，这个价格在1500-3000之间。

第三次我们再折中猜：2250块。

主持人：高了。

1500-2250.

第四次：1875。低了。

1875-2250.

第五次：2062。高了。

1875-2062。

第六次：1968。低了。

1968-2062。

第七次：2015。高了。

1968-2015。

第八次：1991。低了。

1991-2015。

第九次：2003。高了。

1991-2003。

第十次：1997。低了。

1997-2003。

第十一次：2000。答对了！！！

二分的威力，把2000次的搜索空间降到了11次。这也就是时间复杂度中log(n)的来历了。每次都砍掉当前搜索空间的一半，可不就是把原本为n的搜索空间变成了log(n)吗？！

二分的核心思想，很简单，但是难就难在，怎么去实现，或者说，把实际问题巧妙的转化为二分法。

那么现在，我们也清楚了，与二分搜索(binary search)对应的是线性搜索(linear search)。线性搜索对应的时间复杂度就是O(n)。