# Manifesto [![ghit.me](https://ghit.me/badge.svg?repo=cristaloleg/manifesto)](https://ghit.me/repo/cristaloleg/manifesto)
### Git
- 1 commit per change, do squash
  - you can easily work with changes 
- touch few things at once
  - it's kinda obvious
- rebase instead of merge
  - no merge commits, cleaner git history
- pull request must have 2+ approvals
  - changes must be visible to the team members
- master is read-only
  - it's a rule. always. no exclusions.
- delete branches after a merge
  - better navigation and git performance
- release tags
  - tracking releases/deployments are simpler
- git submodules for components
  - better architecture consistency
- no global history changes
  - prevents git history misuse

### CI
- autorevert on failure
  - no broken code in the master
- run at any commit
  - obvious ability for CI
- CI plan in git
  - know all plan changes and have consistency
- warn about formatting verification
  - no developer disruption in the future
- warn about coverage illness
  - coverage is quite important thing
- track test(flakiness) failures
  - statistics, hints, conclusions
- store build logs for 3+ months
  - having analytics and working links to them
- docs are generated from the code
  - end-user changes must be explicit

### Code health
- fork instead of hack
- touch legacy, often
- remove deprecated stuff
- use TODO, BUG, XXX in code
- use linters and code analysis all the time

### Dependencies
- bump libs on a permanent basis
- have a local cache-server with deps
- all modules must have same structure

### Tests
- use one test framework
- show results, not just stacktraces

### Tools
- use Makefile, Bash

### Recovery
- use partial backups
- test your backups

### Team
- pairing, 50% and more
- high-level stand ups, time bounded
- 2-3 week sprints
- per sprint roles
- only urgent topics are face-to-face

### Meetings
- I can skip if I'm out of scope
- if you're organizing a meeting - prepare an agenda

### Communications
- outcomes of important discussions should be on wiki
- only important notifications
- easy access to any team room
- do not delete personal chats with inactive users

### Permissions
- Git, CI, SSH read-access to everything
- one login to anything
- each office should have global admin

### Space
- engineers apart from non-engineers
- quite open-space
- quite zones
- kitchen isn't for chill-out

### Network
- VPN access from home
- Wifi must work all the time
- LAN must be even more stable

### Life
- work from home is a must have
- educational budget to anything related to dev stuff
- allow to commit to the open-source
- skipping team lunch must be acceptable
