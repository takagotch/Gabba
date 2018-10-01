### gabba
---

https://github.com/hybridgroup/gabba

```ruby
Gabba::Gabba.new("UT-1234", "mydomain.com").page_view("something", "track/me")
Gabba::Gabba.new("UT-1234", "mydomain.com").event("Videos", "Play", "ID", "ID", true)
gabba = Gabba::Gabba.new("UT-1234", "mydomain.com")
gabba.identitfy_user(cookies[:__utma], cookies[:__utmz])
gabba.page_view("something", "track/me")

index = 1
scope = Gabba::Gabba::VISITOR
gabba.set_custom_var(index, 'Name', 'Value', scope)
gabba.event(...)
gabba.page_view(...)

index = 1
gabba.delete_custom_var index

g = Gabba::Gabba.new("UT-6666", "myawesomeshop.net")
g.transaction("1234567890", "1000.00", 'Acme Clothing', '1.29', '5.00', 'Los Angeles', 'California', 'USA')
```

