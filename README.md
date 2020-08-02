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

rails g model Comment article:references from:string body:text
rake db:migrate
vi app/models/article.rb
vi app/models/comment.rb
rails c
article = Article.first
article.comments.create(:from => 'rubyist', :body => 'comment1')
article.comments.create(:from => 'rubyist', :body => 'comment2')
article.comments.count
vi app/views/home/index.html.erb
curl http://localhost:3000/
vi app/controllers/home_controller.rb
vi app/views/home/page.html.erb
vi config/routes.rb
vi app/views/home/index.html.erb
curl http://localhost:3000/page/1


vi app/views/home/page.html.erb
vi app/views/home/page.html.erb
vi app/controllers/home_controller.rb
rails g controller comments
vi app/controllers/comments_controller.rb
vi config/routes.rb

vi app/views/home/page.html.erb
vi app/views/comments/_list.html.erb
vi app/views/comments/_form.html.erb
vi app/models/comment.rb
vi app/controller/comments_controller.rb
vi app/views/comments/_from.html.erb
```

```
```

```
curl http://localhost:3000/
curl http://localhost:3000/articles
curl http://localhost:3000/articles/1
curl http://localhost:3000/page/1

```



