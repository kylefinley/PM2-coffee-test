```bash

➜ PM2-coffee-test git:(master) ✗ pm2 --version
0.12.1

➜ PM2-coffee-test git:(master) ✗ pm2 start server.coffee
[PM2] Process server.coffee launched
┌───────────────┬────┬──────┬───────┬─────────┬───────────┬────────┬─────────────┬──────────┐
│ App name      │ id │ mode │ PID   │ status  │ restarted │ uptime │      memory │ watching │
├───────────────┼────┼──────┼───────┼─────────┼───────────┼────────┼─────────────┼──────────┤
│ server.coffee │ 1  │ fork │ 80919 │ online  │         0 │ 0s     │ 10.086 MB   │ disabled │
└───────────────┴────┴──────┴───────┴─────────┴───────────┴────────┴─────────────┴──────────┘

➜ PM2-coffee-test git:(master) ✗ pm2 --version
0.12.2

bash-3.2$ export DEBUG="pm2:*"
bash-3.2$ pm2 start server.coffee --no-daemon
pm2 launched in no-daemon mode (you can add DEBUG="*" env variable to get more messages)
  pm2:satan [PING PM2] Trying to connect to server +0ms
  pm2:satan Daemon alive +11ms
>> pm2 is already daemonized ! You should kill it before launching it in no-daemon mode
  pm2:satan [PING PM2] Trying to connect to server +2ms
  pm2:satan Daemon alive +2ms
  pm2:satan Launching RPC client on port /Users/finley/.pm2/rpc.sock undefined +0ms
  pm2:satan Connected to Daemon +1ms
  pm2:cli Got message from Satan as succesfully connected to PM2, now parsing arguments +5ms
  pm2:satan Calling daemon method pm2:getVersion +1ms
  pm2:monit Before processing +15ms { script: 'server.coffee',
  node_args: undefined,
  max_memory_restart: undefined,
  instances: undefined,
  log_file: undefined,
  error_file: undefined,
  out_file: undefined,
  pid_file: undefined,
  cron_restart: undefined,
  cwd: undefined,
  merge_logs: undefined,
  watch: undefined,
  ignore_watch: undefined,
  env: undefined,
  log_date_format: undefined,
  min_uptime: undefined,
  max_restarts: undefined,
  exec_mode: 'fork_mode',
  exec_interpreter: 'none',
  write: undefined,
  force: undefined,
  post_update: undefined,
  name: 'server' }
  pm2:monit After processing +5ms { errors: [],
  config: 
   { script: 'server.coffee',
     name: 'server',
     exec_mode: 'fork_mode',
     exec_interpreter: 'none' } }
  pm2:monit { script: 'server.coffee', name: 'server', exec_mode: 'fork_mode', exec_interpreter: 'none' } +11ms
  pm2:satan Calling daemon method pm2:findByFullPath +1ms
  pm2:satan Calling daemon method pm2:prepare +22ms
[PM2] Process server.coffee launched
  pm2:monit Getting interaction info +72ms
  pm2:interface:daemon [PING INTERACTOR] Trying to connect to Interactor daemon +0ms
  pm2:interface:daemon Interactor Daemon not launched +110ms
  pm2:satan Calling daemon method pm2:getMonitorData +7ms
┌──────────┬────┬──────┬───────┬────────┬───────────┬────────┬────────────┬──────────┐
│ App name │ id │ mode │ PID   │ status │ restarted │ uptime │     memory │ watching │
├──────────┼────┼──────┼───────┼────────┼───────────┼────────┼────────────┼──────────┤
│ server   │ 2  │ fork │ 81995 │ online │         1 │ 0s     │ 2.422 MB   │ disabled │
└──────────┴────┴──────┴───────┴────────┴───────────┴────────┴────────────┴──────────┘
 Use `pm2 info <id|name>` to get more details about an app
--no-daemon option enabled = do not exit pm2 CLI
PM2 dameon PID = 81226
PM2: 2014-12-23 19:34:35: App name:server id:1 exited
PM2: 2014-12-23 19:34:35: Starting execution sequence in -fork mode- for app name:server id:1
PM2: 2014-12-23 19:34:35: App name:server id:1 online
PM2: 2014-12-23 19:34:35: App name:server id:1 exited
PM2: 2014-12-23 19:34:35: Starting execution sequence in -fork mode- for app name:server id:1
PM2: 2014-12-23 19:34:35: App name:server id:1 online
PM2: 2014-12-23 19:34:35: App name:server id:1 exited
PM2: 2014-12-23 19:34:35: Starting execution sequence in -fork mode- for app name:server id:1
PM2: 2014-12-23 19:34:35: App name:server id:1 online
PM2: 2014-12-23 19:34:35: App name:server id:1 exited
PM2: 2014-12-23 19:34:35: Starting execution sequence in -fork mode- for app name:server id:1
PM2: 2014-12-23 19:34:35: App name:server id:1 online
PM2: 2014-12-23 19:34:36: App name:server id:1 exited
PM2: 2014-12-23 19:34:36: Script /Users/finley/Development/Github/kylefinley/PM2-coffee-test/server.coffee had too many unstable restarts (15). Stopped. "errored"
PM2: 2014-12-23 19:37:56: Process with pid 81841 killed
PM2: 2014-12-23 19:43:06: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:06: App name:server id:2 online
PM2: 2014-12-23 19:43:06: App name:server id:2 exited
PM2: 2014-12-23 19:43:06: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:07: App name:server id:2 online
PM2: 2014-12-23 19:43:07: App name:server id:2 exited
PM2: 2014-12-23 19:43:07: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:07: App name:server id:2 online
PM2: 2014-12-23 19:43:07: App name:server id:2 exited
PM2: 2014-12-23 19:43:07: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:07: App name:server id:2 online
PM2: 2014-12-23 19:43:07: App name:server id:2 exited
PM2: 2014-12-23 19:43:07: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:07: App name:server id:2 online
PM2: 2014-12-23 19:43:07: App name:server id:2 exited
PM2: 2014-12-23 19:43:07: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:07: App name:server id:2 online
PM2: 2014-12-23 19:43:07: App name:server id:2 exited
PM2: 2014-12-23 19:43:07: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:07: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: Proc is not defined anymore or is being killed
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:09: App name:server id:2 exited
PM2: 2014-12-23 19:43:09: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:09: App name:server id:2 online
PM2: 2014-12-23 19:43:09: App name:server id:2 exited
PM2: 2014-12-23 19:43:09: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:09: App name:server id:2 online
PM2: 2014-12-23 19:43:09: App name:server id:2 exited
PM2: 2014-12-23 19:43:09: Script /Users/finley/Development/Github/kylefinley/PM2-coffee-test/server.coffee had too many unstable restarts (15). Stopped. "errored"


➜ PM2-coffee-test git:(master) ✗ pm2 logs
########### Starting streaming logs for [all] process
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:08: App name:server id:2 exited
PM2: 2014-12-23 19:43:08: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:08: App name:server id:2 online
PM2: 2014-12-23 19:43:09: App name:server id:2 exited
PM2: 2014-12-23 19:43:09: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:09: App name:server id:2 online
PM2: 2014-12-23 19:43:09: App name:server id:2 exited
PM2: 2014-12-23 19:43:09: Starting execution sequence in -fork mode- for app name:server id:2
PM2: 2014-12-23 19:43:09: App name:server id:2 online
PM2: 2014-12-23 19:43:09: App name:server id:2 exited
PM2: 2014-12-23 19:43:09: Script /Users/finley/Development/Github/kylefinley/PM2-coffee-test/server.coffee had too many unstable restarts (15). Stopped. "errored"
server-2 (err): SyntaxError: Unexpected string
server-2 (err):     at Module._compile (module.js:439:25)
server-2 (err):     at Object.Module._extensions..js (module.js:474:10)
server-2 (err):     at Module.load (module.js:356:32)
server-2 (err):     at Function.Module._load (module.js:312:12)
server-2 (err):     at Function.Module.runMain (module.js:497:10)
server-2 (err):     at startup (node.js:119:16)
server-2 (err):     at node.js:906:3
server-2 (err): /Users/finley/Development/Github/kylefinley/PM2-coffee-test/server.coffee:1
server-2 (err): tion (exports, require, module, __filename, __dirname) { http = require 'http'
server-2 (err):                                                                         ^^^^^^
server-2 (err): SyntaxError: Unexpected string
server-2 (err):     at Module._compile (module.js:439:25)
server-2 (err):     at Object.Module._extensions..js (module.js:474:10)
server-2 (err):     at Module.load (module.js:356:32)
server-2 (err):     at Function.Module._load (module.js:312:12)
server-2 (err):     at Function.Module.runMain (module.js:497:10)
server-2 (err):     at startup (node.js:119:16)
server-2 (err):     at node.js:906:3
```
