# find-non-translated-keys-resx
Find the keys that are not translated in your .NET resx files.

# How to use it
Clone the repo and execute:

```
npm install
npm run list -- --langs fr,pt,de,es c:\Code\Desktop
```

# How does it work
It looks for every `.resx` in the folder you give, and all the lang variations
you want (in the example above : `.fr.resx`, `.pt.resx`, `.de.resx`, `.es.resx`),
then check if all the keys in the base `.resx` (which is the master language
resource file) exists in the other language (if the file exists).

# Structure expected
```
Settings.resx
Settings.fr.resx
Settings.pt.resx
Settings.de.resx
Settings.en.resx
```

