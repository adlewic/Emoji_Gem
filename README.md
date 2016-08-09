## 😗 Emoji Picker 👆🏼

This gem allows you to integrate a small picker menu of emojis 😎 🙊 👏🏻 to add to your articles / post  and every text field that you want. 😁


##Intallation
Go to you Gemfile on your Rails app  and add this : 
```ruby
gem 'rails_emoji_picker'
```

Then run the command on your terminal : 
```ruby
rails g rails_emoji_picker:install
```

`application.js`
```js
//= require jquery
//= require rails_emoji_picker
//= require_tree .
```


```css
/*
 *= require_tree .
 *= require rails_emoji_picker
 *= require bootstrap
 *= require_self
 */
```



`application.scss or sass`

```scss
@import 'rails_emoji_picker'
```
Next step, wrap your text input with css class `emoji-picker-container`

And add data-attribte `data: { emojiable: true }` to your input/text_area.
```erb
<p class="emoji-picker-container">
  <%= f.text_field :title, class: 'form-control', data: { emojiable: true } %>
</p>
```


