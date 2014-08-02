# pasquale-cli

`$ npm install -g pasquale-cli`

## Usage

```
Checks for spelling errors.
Usage: node ./bin/pasquale --lang=[lang] [text]

Examples:
  node ./bin/pasquale --lang=pt-br istu é errado    Finds errors in pt-br text
  node ./bin/pasquale --default=pt-br               Sets default lang to pt-br


Options:
  -l, --lang              The language to check spelling against                                                                                            [default: "en-ca"]
  -t, --text              The text to have spelling checked against
  -r, --reporter          Specifies which reporter to use                                                                                                   [default: "json"]
  -d, --default           Specifies which lang to be set as default. This
			  one will be saved at the config file
  -i, --ignored           Refers to the list of ignored words. If no other
			  args, lists the ignored words. It might be
			  used with --add, --remove.
  --ri, --remove-ignored  Removes a word from the list of ignored ones
```

## Config

It is also possible to determine a default lang and other config stuff. For doing that, a `.pasqualerc` is needed. Its structure must complain the follow:

```json
{
	"default": "pt-br",
	"ignored": ["palavra1", "palavra2", "palavra3"]
	}
}
```

## Languages

The supported languages (downloadable from [pasquale-inc repo](https://github.com/pasquale-inc)) are the following:

|          name         |  key  |
|-----------------------|-------|
| Català                |       |
| Croatian              |       |
| Dansk                 |       |
| Deutsch               | de    |
| Deutsch (AT)          | de-at |
| Deutsch (CH)          | de-ch |
| Deutsch (DE)          | de-de |
| Czech                 | cs    |
| Ελληνικά              |       |
| English (Canadian)    | en-ca |
| English (British)     | en-gb |
| Español               | es    |
| Français              | fr    |
| Galego                |       |
| Italiano              |       |
| Lietuvių              |       |
| Magyar                |       |
| Nederlands            |       |
| Norwegian (Bokmål)    |       |
| Norwegian (Nynorsk)   |       |
| Română                |       |
| Polski                |       |
| Português (do Brasil) | pt-br |
| Português (Europeu)   | pt    |
| Русский               |       |
| Slovenian             |       |
| Slovensky             |       |
| Svenska               |       |
| Tiếng Việt            |       |
| Українська            |       |

