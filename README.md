# Manifesto [![ghit.me](https://ghit.me/badge.svg?repo=cristaloleg/manifesto)](https://ghit.me/repo/cristaloleg/manifesto)
### Git
- 1 commit per change, do squash
- touch few things at once
- rebase instead of merge
- pull request should have 2+ approvals
- master is read-only
- delete branches after a merge
- release tags
- git submodules for components
- no global stylefixes

### CI
- autorevert on failure
- run at any commit
- CI plan in git
- warn about formatting verification
- warn about coverage illness
- track test(flakiness) failures
- store build logs for 3+ months
- docs are generated from the code

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
