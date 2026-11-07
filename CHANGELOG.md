# What's new

## 0.8

**Hears you better, whoever is speaking**
- Euthus now listens with NVIDIA Parakeet, running on your Mac. In a test with voices from India, the US, the UK and
  South Africa it got 88 of 90 commands and references right, and puts the verse up about a second sooner.
  Apple's recognizer stays available in Settings → Audio, and takes over automatically if Parakeet can't load.
- Voice commands are understood even when they are misheard: "next to us", "next was" or "next, please" → next verse;
  "put this in LLD" → NLT; "put this intelligent" → Telugu; "any SV" → ESV.
- Badly misheard book names are recognised when a chapter and verse follow: "Travers 29 verse 13" → Proverbs 29:13.
- "John 3:16, next verse" and "…verse 3, previous verse" work in one breath, and saying "next verse" three times
  moves three verses.
- Fewer surprises: a command waits until the sentence ends ("Next week we will meet…" no longer moves the verse), and
  verses that only resemble what was said are suggested, never put on screen by themselves.

## 0.7

**Works the same on every Mac**
- A new Mac is ready in seconds. The meaning-search index for the King James Version now comes inside the app,
  instead of being built on first launch (which kept the Mac busy for several minutes and slowed detection and typing).
- Any index that does need building now runs on the Mac's low-power cores, away from speech recognition.
- Apple's speech model downloads when Euthus opens, not when you first press Listen.

**Safer with your files**
- A Bible file Euthus can't read is now listed in Settings → Scripture instead of quietly disappearing.
- A damaged songs, slides or themes file is set aside and kept, never overwritten.
- Imported themes can only use pictures and videos from Euthus's own Backgrounds folder.

**Smoother**
- Customize the toolbar (right-click it). Optional Timer and Outputs buttons.
- The sermon timer survives a restart.
- The Media panel notices new and removed files by itself.
- Type-ahead understands multi-word books and run-together input: `song of sol 2`, `joh3`, `ps23`.
- Settings, Slides and Theme Designer use the system text styles.

## 0.6

First public release: spoken references, quotes and read-along; Preview/Program; up to four outputs with NDI;
confidence monitor; green-key lower third; themes and Media backgrounds; in-app updates.
