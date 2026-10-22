**Holdout audits RL environments and agent evals for reward hacks**: ways an agent can get full reward without doing the task.

For each finding we send a reproduction, the affected tasks, a proposed fix and a regression test. We also build policy-heavy business-workflow environments and hold them to the same test.

- **Findings:** 107 reproduced reward-hack bugs in 20 public repos from 17 organisations, more than 80 not previously reported. Maintainers are told first. Public log: [holdout.cc/findings](https://holdout.cc/findings/)
- **Filed so far:** [PrimeIntellect-ai/verifiers #2947](https://github.com/PrimeIntellect-ai/verifiers/issues/2947) · [PrimeIntellect-ai/verifiers #2948](https://github.com/PrimeIntellect-ai/verifiers/issues/2948) · [NVIDIA-NeMo/Gym #4900](https://github.com/NVIDIA-NeMo/Gym/issues/4900) · [NVIDIA-NeMo/Gym #4901](https://github.com/NVIDIA-NeMo/Gym/issues/4901)
- **Disclosure policy:** [holdout.cc/disclosure](https://holdout.cc/disclosure/)
- **Sample environment:** an accounts-payable exception queue with reference solutions and shortcut strategies that must fail. Repo: [ap-exception-queue](https://github.com/holdout-cc/ap-exception-queue) · [holdout.cc/environments/accounts-payable](https://holdout.cc/environments/accounts-payable/)
- **Sample audit report:** [holdout.cc/audits/sample-report](https://holdout.cc/audits/sample-report/)

Want an environment checked before it ships? [holdout.cc/audits](https://holdout.cc/audits/) · hello@holdout.cc
