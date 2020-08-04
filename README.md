Frozen Record
=============

Frozen record bug using ActiveModel "~> 5.0"

```
bundle install
bundle console

require './payment_icon.rb`
Payment.all.last

irb(main):002:0> PaymentIcon.all.last
Traceback (most recent call last):
       16: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/friendly_errors.rb:123:in `with_friendly_errors'
       15: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/exe/bundle:46:in `block in <top (required)>'
       14: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/cli.rb:24:in `start'
       13: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/vendor/thor/lib/thor/base.rb:476:in `start'
       12: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/cli.rb:30:in `dispatch'
       11: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/vendor/thor/lib/thor.rb:399:in `dispatch'
       10: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/vendor/thor/lib/thor/invocation.rb:127:in `invoke_command'
        9: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/vendor/thor/lib/thor/command.rb:27:in `run'
        8: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/cli.rb:506:in `console'
        7: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/bundler-2.1.4/lib/bundler/cli/console.rb:19:in `run'
        6: from (irb):2
        5: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/frozen_record-0.19.1/lib/frozen_record/scope.rb:11:in `last'
        4: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/frozen_record-0.19.1/lib/frozen_record/scope.rb:61:in `to_a'
        3: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/frozen_record-0.19.1/lib/frozen_record/scope.rb:168:in `query_results'
        2: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/frozen_record-0.19.1/lib/frozen_record/scope.rb:172:in `matching_records'
        1: from /Users/rramsden/.asdf/installs/ruby/2.7.1/lib/ruby/gems/2.7.0/gems/frozen_record-0.19.1/lib/frozen_record/base.rb:153:in `load_records'
NoMethodError (undefined method `values' for nil:NilClass)
```
