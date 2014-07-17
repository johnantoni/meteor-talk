## Meteor Talk Notes (July 16th 2014)

https://twitter.com/joshowens

4 to six weeks build to a polished mvp

Built fantasyhub.com, pulling in stats from mlb, nfl

mini-mongoid tend to use
amazing packaging system, goto differential to see packages...

https://github.com/Differential

built boilerplate (designer maintains)
http://github.com/Differential/meteor-boilerplate

subscription / ddp

integrating cordova into the meteor build, rumour

still a lot of learning for the community on how to build a reactive ui

testing framework wasn't great but it's coming together with Velocity

http://differential.io/blog/what-is-velocity

0.9 coming out, already got jasmine unit testing, cucumber broken, selenium in place, nightwatch (can connect to saucelabs)

reactive testing.

velocity
..has runner which spins up a clone of meteor and runs the tests against a mirror of your data without polluting your real data.
..while your messing with those files it's running those tests for you.

error handling in meteor not as robust as would like to be. should get better in time.

other thing i miss is a something like resque or sidekick. (for our fantasyhub game). did a job fail does it need to be requed.

mongo database being used primarily.

## question time

### process of maintining an app after launch:
..we usually help to hire a team to over it long term, hasn't been that bad, we try to stick to a structure that makes sense. have a document to send over to explain it.
..episodes folder, view folder, map it out across the team. we have an agreed upon structure that others can follow.

### testing:
..velocity, would like a group to make this more aware, writing documentation to help integrate others. how to integrate carnodes.

### load testing:
..not a ton that i know of, adrian lanning, wrote a tool to hammer an app to see what kind of statistics you get on it.
..we were seeing 90% utilization on mongo, then we moved to mongohq and turned and elastic databases and that dropped significantly.

### place where the velocity framework will be:
=> velocity.meteor.com

splitting into 2 groups, second working on galaxy. deploy to meteor.com not supported well, next step up would be heroku, ok option in my mind (still some questions to ask, dynos, but they support mongohq from the get go) so and advantage from modulus. we put most of ours on modulus and when it gets decent traffic we move it to mongohq.

### deploying:
ec2, digitial ocean, own deploys, another one coming called rocker-docker. they're working on a docker solution or a pay-us-to-deploy solution.

### book:

testingwithmeteor.com

book built in middleman, compiled into html, using print to create it.

book on gumroad, put github name in and you'll get access to the repo.
