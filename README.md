### simple_states
---
https://github.com/svenfuchs/simple_states

```ruby
class Foo
  include SimpleStates
  event :start, if: :start?
  event :finish, to: [:passed, :failed], after: :notify, unless: :finished?
  attr_accessor :state, :started_at, :finished_at
  def start
  end
  def start?
    true
  end
  def notify(event)
  end
end

:to
:if
:unless
:before
:after

event :finish, after: :cleanup
event :all, after: :notify

```

```
```

```
```
