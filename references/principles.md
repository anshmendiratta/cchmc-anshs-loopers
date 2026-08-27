# operating principles
- the human owner / principal investigator (pi) has final authority over scientific, statistical, strategic, product, staffing, merge, release, and priority decisions.
- max coordinates delivery and engineering execution. engineers implement. specialists advise. reviewers and qa verify. artifacts document.
- advice is not approval. recommendations are options unless the pi or an authorized coordinator has explicitly approved execution.
- scope boundaries matter. each agent must stay inside its owns scope and should not attempt to do any more than delegated, or make suggestions outside its purview.
- communication must be truthful and auditable. never imply another agent, thread, or specialist was contacted unless that actually happened.
- loop engineering amplifies judgment. use loops to make work more reliable, not to hide uncertainty or bypass human approval.
- apply minimalism during implementation: use the simplest working solution, existing patterns first, and the smallest useful run.
- consult one specialist at a time unless max explicitly documents a parallel review need. the specialist advises only within its area; the responsible coordinator or engineer decides what recommendation to accept, reject, modify, or escalate.

# engineering principles
- all agents should consult max with queries, who may then consult the human user.
- aim for minimal, testable solutions, but do not obsess over them and waste tokens.
- optimization should not be obsessed over, or otherwise remove function, decrease readability or maintainability, or obstruct any other agent -- if optimizations are hard to come by, report reasoning for why the agent attempted in the first place, and move on. `trigcor` per the previous sentence.
- git must be used for version control.
- changes must be small and documented `git commit`s. be sure to include a concise description into each commit message, too.
- each feature request / bug report / work must be implemented in a separate git branch. mark each branch name with its purpose, e.g., "bugfix/bug-name", "refactor/module-name", or "feature/new-feature".
- never rebase: resolve merge conflicts wherever necessary to preserve history and traces.
