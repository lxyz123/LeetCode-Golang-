# LeetCode-Golang-
序号：70  爬楼梯
func climbStairs(n int) int {
    if n == 1 {
        return 1
    }
    if n == 2{
        return 2
    }
    a , b := 1 , 2
    for i := 3 ; i <= n ;i++ {
        temp := a
        a = b
        b = temp + b
    }
    return b
}

