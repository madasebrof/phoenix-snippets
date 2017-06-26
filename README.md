# phoenix-snippets package

Adding Phoenix Snippets to Atom

Updated to swap `=` for `show`, `-` for `wrap`, `#` for `comment`


  `show`
  ```
  <%= $1 %>
  ```

  `wrap`
  ```
  <% $1 %>
  ```

  `comment`
  ```
  <%# $1 %>
  ```

  `for`
  ```
    <%= for ${1:model} <- @${1:model}s do %>
      $2
    <% end %>
  ```

  `et`
  ```
  <%= error_tag ${1:f}, :${1:field} %>
  ```

  `ti`
  ```
  <%= text_input ${1:f}, :${1:field} %>
  ```

  `pi`
  ```
  <%= password_input ${1:f}, :${1:field} %>
  ```

  `lt`
  ```
    <%= link "${1:text}", to: ${2:url} %>
  ```

  `if`
  ```
    <%= if $1 do %>
      $2
    <% end %>
  ```

  `ife`
  ```
    <%= if $1 do %>
      $2
    <% else %>
      $3
    <% end %>
  ```

  `else`
  ```
  <% else %>
  ```

  `unless`
  ```
    <%= unless $1 do %>
      $2
    <% end %>
  ```

  `cond`
  ```
    <%= cond do %>
      <% $1 -> %>
        $2
      <% true -> %>
        $3
    <% end %>
  ```

  `ff`
  ```
    <%= form_for @${1:changeset}, ${2:url}, ${3:[]}, fn f -> %>
      $4
    <% end %>
  ```

  `render`
  ```
    <%= render "${1:partial}.html", ${2:local_var: @local} %>
  ```
