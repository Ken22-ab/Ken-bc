
github
flow-typed / flow-typed / definitions / npm / meow_v3.x.x / test_meow_v3.x.x.js
import meow from 'meow';

const cliBasic = meow('Do stuff');

const cli = meow(`
  Usage
      $ foo <input>

    Options
      -r, --rainbow  Include a rainbow

    Examples
      $ foo unicorns --rainbow
      🌈 unicorns 🌈
`, {
  alias: {
    r: 'rainbow'
  }
});
