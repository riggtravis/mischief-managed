# Mischief Managed
Many of us interact with multiple AWS accounts, roles, profiles, and regions. In
order to avoid accidentally deploying resources to the wrong environment, or
leaving a security vulnerability while leaving a computer briefly unattended
(because trips to the break room for a cup of coffee never are as short as we
plan them to be), just run this script after you've completed whatever task(s)
you needed to connect to a special account for.

Reasons to use Mischief Managed:
1. You've finished a task in your production environment
2. You've been testing something in a sandbox or personal account and want to
  return to the comfort of your default account
3. You need a cup of coffee from the break room

# Why should I use mischief managed instead of some other utility?
Well first of all, mishief managed is a pop culture reference to the biggest
smash hit of the 90s and 00s, Harry Potter. Most other tools don't have that
going for them. The other advantage that mischief managed has over writing your
own script to do this is that I, Travis Rigg, will (probably) continue to add
things that should be cleared out of your environment once you've completed a
sensitive or semi-sensitive task. You can rest safe knowing that I will continue
to add things to this script and you'll just be a git pull away from having an
up to date mischief managed script clearer type thing.

# How do I use Michief Managed
1. Copy `mischief-managed.sh` to a directory on your `PATH`, usually this is a
  folder somewhere named `bin`
2. Make sure `mischief-managed` is executable. You can do this with the
  following command:
```sh
chmod +x mischief-managed
```

## ADVANCED THING DOING
If you're comfortable with symbolic links and want to just keep mischief managed
up to date by running `git pull` you can do the following:

1. Make `mischief-managed` executable as in the steps outlined above.
2. Run the following command:

```sh
ln -s $(pwd)/mischief-managed $HOME/<your place of executables>
```

# How is this script licensed?
I like the MIT license. So it's MIT licensed.