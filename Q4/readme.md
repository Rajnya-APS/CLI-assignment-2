# Question 4

## Aim

To monitor a log file continuously and extract only ERROR messages using Linux command pipelines.

## Description

The command pipeline uses `tail -f` to monitor the log file in real time. The output is passed through `grep` to filter only ERROR messages, which are appended to `report.txt`. Any unwanted error messages are redirected to `/dev/null` using `2>/dev/null`.
