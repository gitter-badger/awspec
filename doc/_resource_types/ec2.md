### exist

```ruby
describe ec2('my-ec2') do
  it { should exist }
end
```

### be_disabled_api_termination

```ruby
describe ec2('my-ec2') do
  it { should be_disabled_api_termination }
end
```

### be_pending

```ruby
describe ec2('my-ec2') do
  it { should be_pending }
end
```

### be_pending, be_running, be_shutting_down, be_terminated, be_stopping, be_stopped

```ruby
describe ec2('my-ec2') do
  it { should be_running }
end
```

### have_ebs

```ruby
describe ec2('my-ec2') do
  it { should have_ebs('vol-123a123b') }
  it { should have_ebs('my-volume') }
end
```

### have_eip

```ruby
describe ec2('my-ec2') do
  it { should have_eip('123.0.456.789') }
end
```

### have_security_group

```ruby
describe ec2('my-ec2') do
  it { should have_security_group('my-security-group-name') }
  it { should have_security_group('sg-1a2b3cd4') }
end
```

### belong_to_subnet

```ruby
describe ec2('my-ec2') do
  it { should belong_to_subnet('subnet-1234a567') }
  it { should belong_to_subnet('my-subnet') }
end
```

### belong_to_vpc

```ruby
describe ec2('my-ec2') do
  it { should belong_to_vpc('vpc-ab123cde') }
  it { should belong_to_vpc('my-vpc') }
end
```
