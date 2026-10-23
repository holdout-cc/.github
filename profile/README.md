**Holdout audits RL environments and agent evals for reward hacks**: ways an agent can get full reward without doing the task.

For each finding we send a reproduction, the affected tasks, a proposed fix and a regression test. We also build policy-heavy business-workflow environments and hold them to the same test.

**Recent outcome:** a reward-file bug we reported in Scale's agentenv-framework ([#305](https://github.com/scaleapi/agentenv-framework/issues/305)) was fixed and merged after our review of the first fix caught a regression that would have broken production verifiers ([#310](https://github.com/scaleapi/agentenv-framework/pull/310)).

- **Findings:** 23 issues filed in public RL environments and benchmarks, including NVIDIA NeMo Gym, Prime Intellect verifiers, Scale, Hugging Face OpenEnv, Toloka, UiPath, HUD and Sierra tau2-bench. 1 is fixed, and 6 more have fix PRs under review. Each one has a Linux reproduction: [holdout-findings](https://github.com/holdout-cc/holdout-findings)
- **Patterns:** 17 recurring ways graders give credit for work that wasn't done, each with a runnable example and a fix: [reward-hack-patterns](https://github.com/holdout-cc/reward-hack-patterns)
- **Sample environment:** an accounts-payable exception queue with reference solutions and shortcut strategies that must fail. Repo: [ap-exception-queue](https://github.com/holdout-cc/ap-exception-queue) · [holdout.cc/environments/accounts-payable](https://holdout.cc/environments/accounts-payable/)
- **Sample audit report:** [holdout.cc/audits/sample-report](https://holdout.cc/audits/sample-report/)
- **Disclosure policy:** [holdout.cc/disclosure](https://holdout.cc/disclosure/)

Want an environment checked before it ships? [holdout.cc/audits](https://holdout.cc/audits/) · hello@holdout.cc
