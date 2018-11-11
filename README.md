### Rbkit
---
https://github.com/code-mancers/rbkit

http://rbkit.codemancers.com/

```
bundle exec
cd <RBKIT_PATH/ext>
ruby extconf.rb
make

cd <RBKIT_PATH>
bundle install
bundle exec rake compile

brew install zeromq
brew install msgpack

gem 'rbkit', path: <RBKIT_PATH>
ruby setup.rb
```

```ruby
require 'rbkit'
Rbkit.start_server

Rbkit.start_server(pub_port: nil, request_port: nil)

Rbkit.start_profiling(
  pub_port: nil, request_port: nil,
  enable_object_trace: true,
  enable_gc_stats: true,
  enable_cpu_profiling: true,
  clock_type: :wall,
  cpu_profiling_mode: :sampling,
  cpu_sampling_interval_usec: 1000
)
```

```
```
