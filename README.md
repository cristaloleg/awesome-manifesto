# Manifesto [![ghit.me](https://ghit.me/badge.svg?repo=cristaloleg/manifesto)](https://ghit.me/repo/cristaloleg/manifesto)

What I would like to see in a company of my dream.

### Git
- [ ] 1 commit per change, do squash
  - you can easily work with changes
- [ ] touch few things at once
  - it's kinda obvious
- [ ] rebase instead of merge
  - no merge commits, cleaner git history
- [ ] pull request must have 2+ approvals
  - changes must be visible to the team members
- [ ] master is read-only
  - it's a rule. always. no exceptions.
- [ ] delete branches after a merge
  - better navigation and git performance
- [ ] release tags
  - tracking releases/deployments are simpler
- [ ] git submodules for components
  - better architecture consistency
  - UPD: highly debatable point
- [ ] no global history changes
  - prevents git history misuse
- [ ] commit message format
  - clear, well explanatory, structured

### CI
- [ ] auto revert on failure
  - roll back a changes, no broken code in the master
- [ ] run at any commit
  - the obvious ability for CI
- [ ] CI plan in git
  - know all plan changes and have consistency
- [ ] warn about formatting verification
  - no developer disruption in the future
- [ ] warn about coverage illness
  - coverage is quite important thing
- [ ] track test failures and flakiness
  - statistics, hints, conclusions
- [ ] store build logs for 3+ months
  - having analytics and working links to them
- [ ] docs are generated from the code
  - end-user changes must be explicit
- [ ] locally reproducible builds
  - re-run part of a job on my local machine

### Code health
- [ ] use linters and code analysis all the time
  - the best handling for the best code
- [ ] fork instead of hack
  - logic isolation at the beginning
- [ ] touch legacy, often
  - it becomes non-legacy faster
- [ ] remove deprecated stuff
  - having a bloated dead code is a mistake
- [ ] use TODO, BUG, XXX in code
  - jumping to the issue tracker can be minimised
- [ ] no experiments in the master
  - use your 20% time as a playground, please

### Dependencies
- [ ] bump libs on a permanent basis
  - the new version is expected to be better
- [ ] have a local cache-server with deps
  - adds stability to the infrastructure
- [ ] all modules must have the same structure
  - similar environment everywhere is a good idea

### Tests
- [ ] use one test framework
  - similar environment is better
- [ ] show results, not just stack traces
  - some failures are obvious with visible result
- [ ] isolated tests
  - use beforeTest and afterTest aggressively
- [ ] TDD
  - it really works
- [ ] measure a code coverage
  - quick and easy way to eliminate bugs  

### Tools
- [ ] use Makefile, Bash
  - simple, easy, well known

### Recovery
- [ ] use partial backups
  - restoring from the 10+Gb file is kinda strange
- [ ] test your backups
  - they might be broken

### Team
- [ ] pairing, 50% and more
  - you're doing better, you're not bored
- [ ] high-level stand-ups, time bounded
  - less info about irrelevant stuff
- [ ] 2-3 week sprints
  - have an achievable sprint goal
- [ ] per sprint roles
  - it's quite comfortable time bounds
- [ ] only urgent topics are face-to-face
  - fewer distractions for unimportant things
- [ ] friendly atmosphere
  - no insulting jokes, no trolling, respectful environment
- [ ] 'coding rockstar'
  - it is a demotivation, not an inspiration

### Meetings
- [ ] I can skip if I'm out of scope
  - do not waste team and own time
- [ ] if you're organising a meeting - prepare an agenda
  - to have a way how to drive a meeting

### Communications
- [ ] use the best apps
  - fast, flexible, pleasurable
- [ ] outcomes of important discussions should be on a wiki
  - better visibility for outcomes
- [ ] only important notifications
  - @all should be rare for irrelevant updates
- [ ] easy access to any team room
  - that's obvious, hey
- [ ] do not delete personal chats with inactive users
  - some chats contains interesting ideas

### Permissions
- [ ] Git, CI, SSH read-access to everything
  - reading server logs cannot cause troubles
- [ ] SSO to anything
  - better organisation of credentials
- [ ] each office should have global admin
  - different timezones are bottleneck

### Space
- [ ] engineers apart from non-engineers
  - fire & ice
- [ ] quiet open-space
  - someone might be sensitive to a noise...
- [ ] quiet zones
  - ...really sensitive
- [ ] the kitchen isn't for chill-out
  - the play room is a thing
- [ ] nothing smelly near working area
  - even coffee/cinamon/mowed grass might irritate

### Network
- [ ] VPN access from home
  - work from home is a cool thing
- [ ] Wifi must work all the time
  - obvious
- [ ] LAN must be even more stable
  - uber-obvious

### Life
- [ ] work from home is a must have
  - family, health, even weather might be a reason
- [ ] educational budget to anything related to dev stuff
  - I would like to learn new technologies, why not?
- [ ] allow committing to the open-source
  - company_karma++
- [ ] skipping team events must be acceptable
  - well...obvious
- [ ] 20% time is a vacation like time
  - creating anything that might help someone is awesome
- [ ] brown bags sessions must be rewarded
  - sharing knowledge is a best way to inspire
- [ ] monthly geek swag <3
  - t-shirt, hoodies and all other stuff
- [ ] health food on the kitchen
  - candies are cool, but I would like to live longer
