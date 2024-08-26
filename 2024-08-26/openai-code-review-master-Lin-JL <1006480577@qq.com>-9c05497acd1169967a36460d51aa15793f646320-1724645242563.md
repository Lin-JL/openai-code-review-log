根据git diff记录可以看出以下变更：

1. 在文件`.github/workflows/main-maven-jar.yml`中：
   - push事件的branch从`master`变更为`master-close`
   - pull_request事件的branch从`master`变更为`master-close`

2. 在文件`.github/workflows/main-remote-jar.yml`中：
   - push事件的branch从`master-close`变更为`master`
   - pull_request事件的branch从`master-close`变更为`master`

根据这些更改，可以看出对于两个workflow文件的触发事件和分支配置进行了调整。这些更改可能是为了更好地与其他代码管理流程或者工作流程相配合，确保正确的触发条件和目标分支。在评审过程中需要确保这些更改是合理的，并不会引入意外行为或逻辑错误。如果这些更改符合预期和设计要求，可以继续审查和推进代码的合并和发布。