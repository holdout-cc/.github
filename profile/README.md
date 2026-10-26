**Holdout audits RL environments and agent evals for reward hacks**: ways an agent can get full reward without doing the task, and correct work that a strict grader rejects.

We are a small team. For each finding we send the maintainers a reproduction, the affected tasks and a proposed fix, normally as a public GitHub issue.

**Outcomes so far**
- **Fixed:** a reward-file bug we reported in Scale's agentenv-framework ([#305](https://github.com/scaleapi/agentenv-framework/issues/305)). An outside contributor, salma2vec, opened fix PR [#310](https://github.com/scaleapi/agentenv-framework/pull/310); Scale revised and merged it.
- **Acknowledged:** a UiPath maintainer reviewed our fix for an agent-writable grader input in coder_eval ([#233](https://github.com/UiPath/coder_eval/issues/233), PR [#237](https://github.com/UiPath/coder_eval/pull/237)) and said it was ready to merge once the remaining vectors had a follow-up issue ([#238](https://github.com/UiPath/coder_eval/issues/238)).

**Open source**
- **Findings:** the issues we have filed in public RL environments, training libraries and evals, with reproduction scripts where available and a status a bot refreshes daily: [holdout-findings](https://github.com/holdout-cc/holdout-findings)
- **Patterns:** 17 recurring ways graders give credit for work that wasn't done, each with a stable ID (RHP-01 to RHP-17), a runnable example and a fix or mitigation: [reward-hack-patterns](https://github.com/holdout-cc/reward-hack-patterns)
- **grader-probe:** tests a reward function or answer checker for false credit and false rejection; can run in your CI as a GitHub Action: [grader-probe](https://github.com/holdout-cc/grader-probe)
- **Checklist:** pre-delivery checks for RL environments, 16 of the 26 linked to a real public grading bug: [rl-env-checklist](https://github.com/holdout-cc/rl-env-checklist)
- **Bug corpus:** real grading bugs as regression tests (buggy grader, fixed grader, and the inputs that tell them apart): [grader-bug-corpus](https://github.com/holdout-cc/grader-bug-corpus)
- **Sample environment:** an accounts-payable exception queue with reference solutions and shortcut strategies that must fail: [ap-exception-queue](https://github.com/holdout-cc/ap-exception-queue)

**More:** [sample audit report](https://holdout.cc/audits/sample-report/) · [disclosure policy](https://holdout.cc/disclosure/)

Want an environment or eval checked before it ships? [holdout.cc/audits](https://holdout.cc/audits/) · hello@holdout.cc
