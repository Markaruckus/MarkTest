# Ruby on Rails Test
## Miss Louise's Class

* Word DOC attached
* Part 1 - multiple choice
  * Answers on page 1 and 2
* Part 2 - quiz coding program
```
$ rails new MySite
$ cd MySite
$/MySite bundle install
$/MySite rails server
$ <ctrl-c>
$/MySite/bin/rails touch app/controllers/pages_controller.rb

class PagesController < ApplicationController
  def show
    render template: "pages/#{params[:page]}"
  end
end

$MySite/config notepad++ routes.rb

rails.application.routes.draw do
  get "/pages/:page" => "pages#show"
end
 
$MySite touch app/views/pages/home.html.erb

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Mark's Ruby home page</title>
  </head>
  <body>
    <h1>Hello Miss Louise</h1>
    <p>My name is Mark ;)</p>
    <p>&copy; <%= Date.today.year %> <a href="http://www.iitcsglobal.com">IITCSGlobal.com</a>.</p>
  </body>
</html>
 
$MySite echo “gem 'bootstrap-sass', '~> 3.3', '>= 3.3.7'” >> gemfile
```
