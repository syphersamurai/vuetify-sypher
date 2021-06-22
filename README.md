
<p align="center">
  <img height="130px"
  src="https://raw.githubusercontent.com/syphersamurai/vuetify-sypher/main/images/icon.png">
</p>

<h1 align="center">vuetify-sypher</h1>
<p align="center">Vuetify sypher extension</p>

`vuetify sypher` is a collection snippet extension for Vuetifyjs in visual studio code.



## Installation

Install through VS Code extensions. Search for `vuetify-sypher`

[Visual Studio Code Market Place: vuetify-sypher ](https://marketplace.visualstudio.com/items?itemName=syphersamurai.vuetify-sypher)

Can also be installed using

````
ext install syphersamurai.vuetify-sypher
````

Now you work more time without pressing `ctrl + space`. But if you find it annoying just disable it.


##  Usage
#### Snippet
You don't need usage example if you are familiar with concept of snippets or you looked up the documentation. But here is an example:

Let's suppose you want to insert Button componenet. For that you have to write full component.

````HTML
<v-btn>buttonText<v-btn>
````

But in `vuetify-sypher` only writing `vBtn` will give you all options available for Button component.

Everything is in camel case and with 'v' prefix which is for Vuetifyjs.

If you want to see list of all available props of a component. Just write `v{component-name}Props`. For example : `vBtnProps`,`vAvatarProps` etc.

If you want to insert a component with all of its props. Just write `v{component-name}WithProps`. This will insert component with all of its props. For example : `vBtnWithProps`, `vAvatarWithProps` etc.

#### Templates
Every component in the Vuetify have additional code to write inside it. For example the `v-btn-toggle` component have `v-btn` inside it. Thats why `vuetify-sypher` provides templates for them.
The syntax of template is pretty easy. `v{component}Template` or `v{component}Template{availableTemplate}`
For example `vBtnToggleTemplate` will give you following code.

```HTML
<v-btn-toggle mandatory multiple v-model="value">
  <v-btn flat>
    <v-icon>icon</v-icon>
  </v-btn>
  <v-btn flat>
    <v-icon>icon</v-icon>
  </v-btn>
  <v-btn flat>
    <v-icon>icon</v-icon>
  </v-btn>
  <v-btn flat>
    <v-icon>icon</v-icon>
  </v-btn>
</v-btn-toggle>
```

and `vBtnToggleTemplateTextIcon` will give you following code.
````HTML
<v-btn-toggle multiple mandatory v-model="value">
  <v-btn flat value="value">
    <span>text</span>
    <v-icon>icon</v-icon>
  </v-btn>
  <v-btn flat value="value">
    <span>text</span>
    <v-icon>icon</v-icon>
  </v-btn>
  <v-btn flat value="value">
    <span>text</span>
    <v-icon>icon</v-icon>
  </v-btn>
  <v-btn flat value="value">
    <span>text</span>
    <v-icon>icon</v-icon>
  </v-btn>
</v-btn-toggle>
````


## Questions
If you have any questions, ideas or you want to discuss with me. Just raise a issue in `vuetify-sypher` [github repository](https://github.com/syphersamurai/vuetify-sypher/issues).


## License
[MIT](https://github.com/syphersamurai/vuetify-sypher/blob/master/LICENSE)
