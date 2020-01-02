# Manifesto

### Git
- [ ] 1 commit per change, do squash on merge
  - you can easily work with changes
- [ ] there might be few (already squashed) commits in a pull request
  - don't make huge changes they will bury the truth
- [ ] touch few things at once
  - it's kinda obvious
- [ ] rebase instead of merge
  - no merge commits, cleaner git history
- [ ] pull request must have at least 1-2 approvals
  - changes must be visible to the team members
- [ ] master is read-only
  - it's a rule. Always. No exceptions.
- [ ] delete branches after a merge
  - better navigation and git performance
- [ ] use SemVer as a standard for versioning
  - do not reinvent the wheel
- [ ] release tags
  - tracking releases/deployments are simpler
- [ ] omit release branches for patches (aka 0.1.x)
  - use release tags for that
- [ ] no global history changes
  - prevents git history misuse
- [ ] commit message format
  - clear, well explanatory, structured
- [ ] no big binary files inside a repo
  - slowdowns without a reason
- [ ] have a meaningful README
  - so everyone can quickly get an overview of the repo

### CI
- [ ] auto-revert on failure
  - rollback changes, no broken code in the master
- [ ] run at any commit
  - the obvious ability for CI
- [ ] CI plan in git
  - know all plan changes and have consistency
- [ ] warn about formatting verification
  - no developer disruption in the future
- [ ] warn about coverage illness
  - coverage is a quite important thing
- [ ] track test failures and flakiness
  - statistics, hints, conclusions
- [ ] store build logs for 3+ months
  - having analytics and working links to them
- [ ] do not remove builds/PR/issues
  - unexpected 404 will help no one, will not save disk space also
- [ ] docs are generated from the code
  - end-user changes must be explicit
- [ ] locally reproducible builds
  - re-run part of a job on my local machine
- [ ] use Makefile, Bash
  - simple, easy, well known
- [ ] ability to start/stop a job on CI
  - waiting for an approval to make this action is a horrible bottleneck
- [ ] CI jobs should be runned periodically
  - to reduce possible errors due to hidden dependecies
  
### Deploy
- [ ] configuration files must be validated before a start
  - unless difficult debug is your goal
- [ ] store config in the same repo as a code
  - this prevents 'the chick or the egg' problem
- [ ] all features must be protected by feature flag
  - in case of an accident, it will(might) be enough to turn it off
- [ ] deployment of a new config must be isolated
  - to separate different machines/containters/storages from each other
- [ ] deploy must go from a (git-)tag or release, not from the master
  - this restricts a changeset which will be deployed

### Code health
- [ ] leave your code better than you found it
- [ ] document your code
  - giving a small context for API will save a lot of time
- [ ] use linters and code analysis all the time
  - the best handling for the best code
- [ ] touch legacy, often
  - it becomes non-legacy faster
- [ ] remove deprecated stuff
  - having a bloated dead code is a mistake
- [ ] also remove old code
  - it adds even fewer reasons to the new code
- [ ] use TODO, BUG, XXX in code
  - jumping to the issue tracker can be minimised
- [ ] no experiments in the master
  - use your 20% time as a playground, please
- [ ] allow changing log-level on the fly
  - this will simplify production's debug routine
- [ ] limit your log file, 'cause it might grow unlimited
  - this might cause troubles to your app, be careful
- [ ] store your config in /etc/myapp and logs in /var/log/myapp
  - this will make everything more structured and well defined
- [ ] all modules must have the same structure
  - similar environment everywhere is a good idea
- [ ] if you can’t show a bottleneck, don’t start to optimise it
  - it might be interesting and challenging, but useless
- [ ] check back compatibility before the new releases
  - make it explicit and obvious (+doc how to port)

### Database
- [ ] think about your data
  - don't use SQL/NoSQL without a reason
- [ ] keep models normalized
  - less storage, better performance
- [ ] but don't normalize without a reason
  - everything is a trade off
- [ ] use timestamp to store a date/time
  - this will save you from formatting hell
- [ ] log slow queries
  - see what is happening in a database and who is too greedy
- [ ] don't put business logic into DB or at least make it loosely coupled
  - this will give you an easy migration to another DB

### Dependencies
- [ ] wrap any dependency with an interface(or analogue)
  - this will prevent a vendor lock on it
- [ ] bump libs on a permanent basis
  - the new version is expected to be better
- [ ] have a local cache-server with dependencies
  - adds stability to the infrastructure
- [ ] pin your dependencies to a specific version
  - accidental commit to dependency's master will break nothing
- [ ] prefer mature technology, rather than a hyped one
  - mature will die slower, then hyped
- [ ] fork instead of hack
  - it might be better to fix a lib instead of wrapping for the desired behaviour

### Tests
- [ ] use one test framework
  - a similar environment is better
- [ ] show results, not just stack traces
  - some failures are obvious with visible result
- [ ] isolated tests
  - use beforeTest and afterTest aggressively
- [ ] TDD
  - it really works
- [ ] measure a code coverage
  - a quick and easy way to eliminate bugs  
- [ ] test your backups
  - they might be broken
- [ ] do not hard code ports in tests
  - unless you're interested in random flaky tests

### Team
- [ ] pairing, 50% and more
  - you're doing better, you're not bored
- [ ] high-level stand-ups, time bounded
  - less info about irrelevant stuff
- [ ] 2-3 week sprints
  - have an achievable sprint goal
  - UPD: depends on team/project, might be unuseful
- [ ] per sprint roles
  - it's quite comfortable time bounds
- [ ] only urgent topics are face-to-face
  - fewer distractions for unimportant things
- [ ] friendly atmosphere
  - no insulting environment, respectful trolling
- [ ] 'coding rockstar'
  - it is a demotivation, not an inspiration
- [ ] if you're on the vacations - specify a date range
  - it'll be easier to find someone else or postpone the question
- [ ] FAQ for newcomers
  - 30-day plan with all stuff that they should accomplish
- [ ] document solved and unresolved problems
  - team members will be aware of some problems and it will be resolved much faster
- [ ] every ticket in progress must have an assignee
  - this prevents doing same work on one task 
- [ ] there must be a run book or guide for every responsibility
  - 30/60/90 days plan for newcomers, guide for on call, support

### Meetings
- [ ] I can skip if I'm out of scope
  - do not waste team and own time
- [ ] if you're organising a meeting - prepare an agenda
  - to have a way how to drive a meeting
- [ ] action points after the meeting
  - who does what and when
- [ ] avoid bus factor as much as possible
  - moving/cancelling an unimportant meeting because 1 person is a bad sign

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
  - some chats contain interesting ideas
- [ ] closed ticket must contain a link to the changes
  - every change must be easily accessible and visible for others

### Permissions
- [ ] Git, CI, SSH read-access to everything
  - reading server logs cannot cause troubles
- [ ] SSO to anything
  - better organisation of credentials
- [ ] each office should have global admin
  - different time zones are a bottleneck

### Space
- [ ] engineers apart from non-engineers
  - fire & ice
- [ ] quiet open-space
  - someone might be sensitive to noise...
- [ ] quiet zones
  - ...really sensitive
- [ ] the kitchen isn't for chill-out
  - the playroom is a thing
- [ ] nothing smelly near working area
  - even coffee/cinnamon/mowed grass might irritate

### Network
- [ ] VPN access from home
  - work from home is a cool thing
- [ ] Wifi must work all the time
  - obvious
- [ ] LAN must be even more stable
  - uber-obvious

### Life
- [ ] how often should my salary be reviewed?
  - worth asking
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
  - sharing knowledge is the best way to inspire
- [ ] monthly geek swag <3
  - t-shirts, hoodies and all other stuff
- [ ] health food in the kitchen
  - candies are cool, but I would like to live longer
