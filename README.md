# Ember CLI datepicker

[![Build Status](https://travis-ci.org/soulim/ember-cli-bootstrap-datepicker.svg?branch=master&style=flat)](https://travis-ci.org/soulim/ember-cli-bootstrap-datepicker)

The addon provides you a `bootstrap-datepicker` input component. It can be used in Ember CLI applications.

The input component is based on [bootstrap-datepicker library](https://github.com/eternicode/bootstrap-datepicker).

## Installation

If you are using Ember CLI 0.1.5 and higher, just run within your project directory:

```bash
ember install:addon ember-cli-bootstrap-datepicker
```

When your Ember CLI version is below 0.1.5, please run within your project directory:

```bash
npm install --save-dev ember-cli-bootstrap-datepicker
ember generate bootstrap-datepicker
```

## Usage

Basic example:

```handlebars
{{bootstrap-datepicker value=expiresAt}}
```

The component supports many options of the bootstrap-datepicker library. Let me show you how to use them :sparkles:

### Available options

#### autoclose

Type: `Boolean`
Default: `false`

```handlebars
{{bootstrap-datepicker value=expiresAt autoclose=true}}
```

#### calendarWeeks

Type: `Boolean`
Default: `false`

```handlebars
{{bootstrap-datepicker value=expiresAt calendarWeeks=true}}
```

#### clearBtn

Type: `Boolean`
Default: `false`

```handlebars
{{bootstrap-datepicker value=expiresAt clearBtn=true}}
```

#### daysOfWeekDisabled

Type: `Array` or `String`
Default: `""` or `[]`

```handlebars
{{bootstrap-datepicker value=expiresAt daysOfWeekDisabled="1,2"}}
```

#### endDate

Type: `Date` or `String`
Default: `Infinity` (end of time)

```handlebars
{{bootstrap-datepicker value=expiresAt endDate="01/01/2018"}}
```

#### forceParse

Type: `Boolean`
Default: `true`

```handlebars
{{bootstrap-datepicker value=expiresAt forceParse=false}}
```

#### format

Type: `String`
Default: `'mm/dd/yyyy'`

```handlebars
{{bootstrap-datepicker value=expiresAt format="dd.mm.yy"}}
```

#### keyboardNavigation

Type: `Boolean`
Default: `true`

```handlebars
{{bootstrap-datepicker value=expiresAt keyboardNavigation=false}}
```

#### language

Type: `String`
Default: `'en'`

When you need another language, you should import a locale file using your Brocfile.js. Just import `bower_components/bootstrap-datepicker/js/locales/bootstrap-datepicker.<LANGUAGE_CODE>.js`, e.g.:

```javascript
// Brocfile.js
app.import('bower_components/bootstrap-datepicker/js/locales/bootstrap-datepicker.de.js');
```
```handlebars
{{! somewhere in template }}
{{bootstrap-datepicker value=expiresAt language="de"}}
```

#### minViewMode

Type: `Number` or `String`
Default: `0` or `'days'`

```handlebars
{{bootstrap-datepicker value=expiresAt minViewMode="months"}}
```

#### orientation

Type: `String`
Default: `'auto'`

```handlebars
{{bootstrap-datepicker value=expiresAt orientation="right"}}
```

#### startDate

Type: `Date` or `String`
Default: `-Infinity` (beginning of time)

```handlebars
{{bootstrap-datepicker value=expiresAt startDate="01/01/2014"}}
```

#### startView

Type: `Number` or `String`
Default: `0` or `'month'`

```handlebars
{{bootstrap-datepicker value=expiresAt startView="decade"}}
```

#### todayBtn

Type: `Boolean`
Default: `false`

```handlebars
{{bootstrap-datepicker value=expiresAt todayBtn=true}}
```

#### todayHighlight

Type: `Boolean`
Default: `false`

```handlebars
{{bootstrap-datepicker value=expiresAt todayHighlight=true}}
```

#### weekStart

Type: `Number`
Default: `0` (Sunday)


```handlebars
{{bootstrap-datepicker value=expiresAt weekStart=1}}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## License

[MIT License](https://github.com/soulim/ember-cli-bootstrap-datepicker/blob/master/LICENSE.md)