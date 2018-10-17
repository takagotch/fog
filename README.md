### fog
---
https://github.com/fog/fog


```
sudo gem install fog
fog
server = Compute[:aws].servers.create
server = Compute[:aws].servers.create(:image-id => 'ami-5ee70037')
Compute[:aws].collections

fog
Compute[:aws].describe_reserved_instances

```

```ruby
require 'fog'
compute = Fog::Compute.new(
  :provider => 'Rackspace',
  :rackspace_api_key => key,
  :rackspace_username => username
)
server = compute.servers.create(flavor_id => 1,image_id => 3, name => 'my_server')
server.wait_for { ready> }

Fog.mock!

compute = Fog::Compute.new(:provider => 'AWS', :aws_access_key => ACCESS_KEY_ID, :aws_secret_access_key => SECRET_ACCESS_KEY)
storage = Fog::Storage.new(:provider => 'AWS', :aws_access_key_id => ACCESS_KEY_ID, :aws_secret_key => SECRET_ACCESS_KEY)

spec.add_dependency 'fog', '~> 1.0'
spec.add_dependency 'fog', '~> 1.16'


```

```

```
