# dectl
The dectl is a local continous integration tools for code pulling, building, packaging and deploying.

## Problems always happened after code commited
1. As a developer in a team, The largest problem is that we would meet some merge/conflicts when we commit our changes to the respositry, even if there were no conflicts after merge, we still have to run all the test cases and make sure that these changes won't go wrong before we push.

2. There are plenty of micro-services in a project. We want make itergration earlier to find out some bugs in a stable environment rather than just push ours code to the repository to trigger the Public CI, It will take long times to run all the test cases and if there are some problems, we should revert the changes. In this situration, we couldn't know which micro-services made these problems, currently or previously changes pushed by other developers. This is the value of continous intergration. but, It's not easy to find them out.

3. Is it necessary to build local continuous intergration testing environments by myself? The answer is YES to me. I am going to enjoy a cup of coffee when I pushed my changes, and review report of auto testing results, I have confidence to locate problems in my recent changes, I will fix these problems/bugs by myself, I wouldn't let them to distube other develpers.

## About Workflow
