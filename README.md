# git-commitizen
git 提交规范实践（全局提交很方便，局部提交要找文件麻烦）直接souretree手动输入规范
Git commit日志基本规范
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>

对格式的说明如下：

type代表某次提交的类型，比如是修复一个bug还是增加一个新的feature。所有的type类型如下：
feat： 新增feature
fix: 修复bug
docs: 仅仅修改了文档，比如README, CHANGELOG, CONTRIBUTE等等
style: 仅仅修改了空格、格式缩进、都好等等，不改变代码逻辑
refactor: 代码重构，没有加新功能或者修复bug
perf: 优化相关，比如提升性能、体验
test: 测试用例，包括单元测试、集成测试等
chore: 改变构建流程、或者增加依赖库、工具等
revert: 回滚到上一个版本


Install commitizen globally, if you have not already.

npm install -g commitizen
Install your preferred commitizen adapter globally, for example cz-conventional-changelog

npm install -g cz-conventional-changelog
Create a .czrc file in your home directory, with path referring to the preferred, globally installed, commitizen adapter

echo '{ "path": "cz-conventional-changelog" }' > ~/.czrc
You are all set! Now cdinto any git repository and use git cz instead of git commit and you will find the commitizen prompt.

Protip: You can use all the git commit options with git cz, for example: git cz -a.

