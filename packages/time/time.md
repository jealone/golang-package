# time包
> import “time”

## 概述
time包用于提供计算和展示时间功能

## 目录

### 用例

### 包文件

## 常量
```
`const (
ANSIC       = "Mon Jan \_2 15:04:05 2006"
UnixDate    = "Mon Jan \_2 15:04:05 MST 2006"
RubyDate    = "Mon Jan 02 15:04:05 -0700 2006"
RFC822      = "02 Jan 06 15:04 MST"
RFC822Z     = "02 Jan 06 15:04 -0700" // RFC822 with numeric zone
RFC850      = "Monday, 02-Jan-06 15:04:05 MST"
RFC1123     = "Mon, 02 Jan 2006 15:04:05 MST"
RFC1123Z    = "Mon, 02 Jan 2006 15:04:05 -0700" // RFC1123 with numeric zone
RFC3339     = "2006-01-02T15:04:05Z07:00"
RFC3339Nano = "2006-01-02T15:04:05.999999999Z07:00"
Kitchen     = "3:04PM"
// Handy time stamps.
Stamp      = "Jan \_2 15:04:05"
StampMilli = "Jan \_2 15:04:05.000"
StampMicro = "Jan \_2 15:04:05.000000"
StampNano  = "Jan \_2 15:04:05.000000000"
)
```
`以上预定义的模板，是用于函数`Time.Format`和`Time.Parse`中模板中的引用的时间:
> Mon Jan 2 15:04:05 MST 2006
该时间是时间戳为 1136239445，时间的时区为GMT-0700,引用时间也可以认为是：
> 01/02 03:04:05PM '06 -0700
定义自己的时间格式，

