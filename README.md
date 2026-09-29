# GoPay UI Components

17 UI components fetched from [uiverse.io](https://uiverse.io) for the GoPay (Revolut-like) app.
Each folder contains:
- `index.html` — standalone preview of the component (original markup, CSS inlined in `<style>`)
- `style.css` — the component's raw CSS, extracted verbatim

All code is the original authors' work, preserved as-is. `social-media-ceo` additionally
includes the CEO's real social links (Instagram, X/Twitter, WhatsApp) appended to the markup.

| # | Component | Folder | Source |
|---|-----------|--------|--------|
| 1 | Pay Now button | `pay-now` | https://uiverse.io/fthisilak/bitter-termite-36 |
| 2 | Dark/Light mode toggle | `dark-light-mode` | https://uiverse.io/RiccardoRapelli/jolly-chicken-91 |
| 3 | Social media of CEO founder | `social-media-ceo` | https://uiverse.io/PapaUiiss404/honest-ape-75 |
| 4 | Sent money — success message | `sent-money-success` | https://uiverse.io/akshat-patel28/quick-baboon-29 |
| 5 | Sent money — failed message | `sent-money-failed` | https://uiverse.io/akshat-patel28/fresh-lizard-63 |
| 6 | Sent money — insufficient balance ("Your balance is not enough") | `sent-money-insufficient` | https://uiverse.io/akshat-patel28/tough-octopus-19 |
| 7 | Save card details | `save-card-details` | https://uiverse.io/Peary74/kind-cougar-54 |
| 8 | Add new card | `add-new-card` | https://uiverse.io/nazar-gavrylyk/slippery-snake-30 |
| 9 | Go back button | `go-back` | https://uiverse.io/AKAspidey01/orange-donkey-78 |
| 10 | Send money to user | `send-money-to-user` | https://uiverse.io/marcelodolza/fat-zebra-11 |
| 11 | Login form | `login` | https://uiverse.io/micaelgomestavares/dull-walrus-66 |
| 12 | Pattern | `pattern` | https://uiverse.io/SelfMadeSystem/sweet-dolphin-36 |
| 13 | Card info (press card to view information) | `card-info` | https://uiverse.io/Praashoo7/black-lizard-62 |
| 14 | Home page | `home-page` | https://uiverse.io/byllzz/rude-bat-50 |
| 15 | Loading animation | `loading` | https://uiverse.io/mobinkakei/grumpy-turtle-41 |
| 16 | Contacts support | `contacts-support` | https://uiverse.io/eraly_2449/ancient-bulldog-23 |
| 17 | Navigation bar (blue glass) | `navigation-bar` | https://uiverse.io/mymiamo/yellow-rattlesnake-26 |

## Extraction method

Each uiverse.io page embeds the component code as schema.org `SoftwareSourceCode`
JSON-LD inside a `<meta type="application/ld+json" script="...">` tag. The `text`
field holds `<!-- HTML -->` + `<!-- CSS -->` sections, which were split and saved
verbatim (see `extract.py` for the reusable script).
