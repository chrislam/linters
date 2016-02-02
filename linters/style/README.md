# Stylelint Config Standard

> The standard shareable config for stylelint at Gladeye

Use it as is or as a foundation for your own config.

It is derived from the common rules found within [stylelint-config-standard](https://github.com/stylelint/stylelint-config-standard)

It favours flexibility over strictness for things like multi-line lists and single-line rulesets, and tries to avoid potentially divisive rules.

## Installation

#### System wide

Running this command will place the `.stylelintrc` file in your home folder, and will act as a system wide rules

```
npm install -g stylelint
curl https://raw.githubusercontent.com/gladeye/linters/master/linters/style/.stylelintrc > ~/.stylelintrc
```

#### Per project

Place this [.stylelintrc](https://raw.githubusercontent.com/gladeye/linters/style/.stylelintrc) at the root of your project folder

## Policy

You are allowed to add more rules, or bring down severity of the existing rules (e.g from `error` to `warn`), but you are not **allowed** to remove any existing rules.

## Integration

#### Sublime Text

- Make sure you have `stylelint` executable either in your project by `npm install stylelint` or global by `npm install -g stylelint`

- Install `SublimeLinter` via Package Control

- Install `SublimeLinter-contrib-stylelint` via Package Control

    1.Within Sublime Text, bring up the Command Palette and type install. Among the commands you should see Package Control: Install Package. If that command is not highlighted, use the keyboard or mouse to select it. There will be a pause of a few seconds while Package Control fetches the list of available plugins.

    2.When the plugin list appears, type `stylelint`. Among the entries you should see `SublimeLinter-contrib-stylelint`. If that entry is not highlighted, use the keyboard or mouse to select it.

#### Atom

- Follow instruction [here](https://atom.io/packages/linter-stylelint)

> Note: The Atom package doesn't support global `stylelint` executable, you must have `stylelint` node package included in your project

## Links

- [stylelint](https://github.com/stylelint/stylelint)
- [Rules Documentation](https://github.com/stylelint/stylelint/blob/master/docs/user-guide/rules.md)
