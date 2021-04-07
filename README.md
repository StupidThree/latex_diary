# latex_diary

# DONE
- 年历  
  存在日历的日期会突出显示。  
  点击月份可跳转月历，点击日期可跳转日历。
- 月历  
  可为每一天添加事件。  
  点击日期小编号会跳转到当天的日历。
- 日历  
  左上角显示当月月历，点击可跳转到其他日期。  
  修改`courses.tex`实现课程表导入。  
  ~~抄了一份~~带标记功能的ToDoList。
- 侧栏  
  除年历页外，每页均有右侧栏，可跳转各月月历。
- 底栏  
  每页均有底栏，可跳转各分区（目前只做了Calendar)。

## TODO
- Yearly Plan
- Habit Tracking
- Reading Record
- Movie Record

## 使用
1. 编译  
   编译`calendar.tex`文件生成完整日程本，也可单独编译月历/日历。
2. 新建月历  
   - 复制`2021-04.tex`，修改文件名和文件中`\def\mymonth{04}`的`04`为目标月份。
   - 使用`\csdef{cal-2021-04-03}{event}`的格式修改日程内容。
3. 新建日历  
   - 复制`2021-04-04.tex`，修改文件名和文件中`\def\mymonth{04}`及`\def\myday{04}`为目标月份和日期。
   - 修改各个`\def`填写日历。
4. 修改年份  
   - 修改`beginfile.tex`中`\def\myyear{2021}`为目标年份。
5. 修改课程表  
   - 在`courses.tex`中绘制课程表，并在日历文件中`\def\TodayClasses{}`使用固定的课程表（为方便调休没有做按照星期几自动生成的）。
   
----

我觉得我现在是真的懂了一些Latex……
