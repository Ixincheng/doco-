# doco-
1、问题1：#时间戳过期
ValueError at /admin/login/
timestamp out of range for platform time_t
解决方案：
将# SESSION_COOKIE_AGE = 60 * 60 * 24 * 10000改为：
SESSION_COOKIE_AGE = 60 * 60 * 24
