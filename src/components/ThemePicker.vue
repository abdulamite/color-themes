<!--
  This is where the list of themes lives!

  If you're adding a theme, make sure you've also added the theme
  color variables to ../assets/themes.css

-->

<!--
  Please add your new theme to the end of the list of themes!

  Properties of <Theme> Components:

  - theme-name => this is where you'll add the css class to be applied when selected
  - display-name => The name to display on the Theme Picker Element
  - contributor => github username of contributor [If left blank, default github image will be used instead]

  Note: The theme-name property on Theme components must be the same as the class name added in themes.css
  If no display-name propery is set, the theme-name will be displayed instead.
-->

<template>
  <div id="picker">
    <h1 class="secondary-text">
      Choose a
      <wbr>new theme
    </h1>
    <Theme theme-name="default-light" display-name="Default Light" contributor="12vanblart"/>
    <Theme theme-name="default-dark" display-name="Default Dark" contributor="12vanblart"/>
    <Theme theme-name="roseGold" display-name="Rose Gold" contributor="stroudn1"/>
    <Theme theme-name="fish-finger" display-name="Fishfinger" contributor="iamjinme"/>
    <Theme theme-name="forest-theme" display-name="Forest Theme" contributor="ewenearle"/>
    <Theme theme-name="arduino-theme" display-name="Arduino Theme" contributor="babel78"/>
    <Theme theme-name="morning-blue" display-name="Morning Blue" contributor="chinmay81098"/>
    <Theme theme-name="bubblegum" display-name="Bubblegum" contributor="heatherpekrul"/>
    <Theme theme-name="dracula" display-name="Dracula" contributor="SpaceLenore"/>
    <Theme theme-name="purple-haze" display-name="Purple Haze" contributor="CariZa"/>
    <Theme theme-name="planet-express" display-name="Planet Express" contributor="kylerits" />
    <Theme theme-name="coder" display-name="Coder Theme" contributor="ashishohri"/>
    <Theme theme-name="soft-haze" display-name="Soft Haze Theme" contributor="rebz"/>
    <Theme theme-name="light-dark" display-name="Light Dark" contributor="natandias"/>
    <Theme theme-name="gameboy" display-name="Gameboy" contributor="morsecodemedia"/>
    <Theme theme-name="dark-blue" display-name="Blue" contributor="max003003003"/>
    <Theme theme-name="blue-theme" display-name="Blue Theme" contributor="lupecio"/>
    <Theme theme-name="simple-blue" display-name="Simple Blue Theme" contributor="abdulamite"/>
  </div>
</template>

<script>
import Theme from "./Theme.vue";
export default {
  name: "ThemePicker",
  components: {
    Theme
  }
};
</script>

<style lang="scss" scoped>
#picker {
  background-color: var(--accent);
  text-align: center;
  height: 50vh;
  overflow-y: scroll;
  padding: 0 100px;
}

.secondary-text {
  background-color: var(--secondary);
}

#picker > button:not(:last-of-type) {
  margin-right: 10px;
}

@media screen and (max-width: 600px) {
  #picker > button:not(:last-of-type) {
    margin-right: 0;
  }
}
</style>
