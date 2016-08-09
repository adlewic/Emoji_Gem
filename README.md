## 😗 Emoji Picker 👆🏼

This gem allows you to integrate a small picker menu of emojis 😎 🙊 👏🏻 to add to your articles / post  and every text field that you want. 😁


## Intallation
Go to you `Gemfile` and add the next: 
```ruby
gem 'rails_emoji_picker'
```

Then run the command on your terminal : 
```ruby
rails g rails_emoji_picker:install
```

Go to your file `application.js` and add the following:

```js
//= require jquery
//= require rails_emoji_picker
//= require_tree .
```

Now go to your file `application.css` and add the following:
```css
/*
 *= require_tree .
 *= require rails_emoji_picker
 */
```
If you are using bootstrap  you also have to add the following:
```css
/*
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


