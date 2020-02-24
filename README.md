# LogAppender｜模拟日志生成器

## 简介
这一简单的Java实现可根据传入参数（每次写入行数、写入间隔时间）将样本日志中的特定
行块追加至目标日志中，以模拟日志生成，供后续实时处理。

仅供测试，用了BufferedWriter但实际并未缓存，立即写入。

## 使用

`
javac LogAppender.java
`

`
java LogAppender [日志源] [目标文件] [每次追加的行数] [时间间隔（秒）]
`

---

## Intro
This simple Java implementation is capable of appending specific block
of lines into target log file based on given number of lines and time 
interval to better simulate log appending process, which provides a 
streaming file source for real-time log processing.

For Testing only, BufferedWriter is used but no buffer is actually
exist, the data's written to the file immediately.

## Usage
`
javac LogAppender.java
`

`
java LogAppender [LOG_SRC_PATH] [LOG_TARGET_PATH] [NUMBER_OF_LINES_EACH_CYCLE] [TIME_INTERVAL in seconds]
`
