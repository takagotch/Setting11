### Settings11
---


```
rails new b2 --skip-bundle
cd b2
cat Gemfile
bundle install --path vendor/bundle
rails s
curl https://localhost:3000/
Ctrl + c

rake db:create
rails g scaffold Article title:string content:text
rake db:migrate
curl http://localhost:3000/articles

rails g controller home index
vi app/controllers/home_controller.rb
vi app/views/home/index.html.erb
vi config/routes.rb
rm -rf public/index.html
curl http://localhost:3000/home/index

```

```
```

```
```



