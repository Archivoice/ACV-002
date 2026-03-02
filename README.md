# ACV-002
public voiced acted female (MTF) singing voice dataset

# Dataset Info:
## About The Voice:
Like [ACV-001](https://github.com/Archivoice/ACV-001), this dataset is recorded by Jonathan Huang. However, this dataset is recorded in a feminine voice, or a MTF vocal, so to speak. While Jonathan is not transgender himself, it should be noted that the affects of testosterone are permenant, and HRT would have no affect on the outcome of this dataset.

## Format and Specs:
The dataset is manually labeled with the following systems (the native/non native refers to level of fluency):
>[Mandarin Chinese](https://github.com/Archivoice/AV-diffsinger-Chinese-support) (language tag: `cn/`, native)\
arpabet for English (language tag: `en/`, native)

The dataset labels are generated via [WFL](https://github.com/MLo7Ghinsan/WFL-ASR) and manually corrected.\
Overall, all labels have been manually checked and should be correct, save for a few incorrectly labeled phonemes.

To train exclusively in specific language, you can use tools such as [notepad++](https://notepad-plus-plus.org/downloads/) to search for `/` in the files via the "Find in Files" function.
Which will make a list showing every sample that has a language tag.

The dataset is recorded at 16 bit 44.1k Hz in wav format and labeled in HTK label format (.lab).\
Audio has been dereverbed and denoised for more even consistency.

The dataset is released with two versions, full length and segmented.\
The full length dataset only includes wav and lab files, whereas the segmented dataset includes ds files and a transcription.csv for [diffsinger](https://github.com/openvpi/DiffSinger) usage.\
The ds contains f0 and note slur data.

## Additional Info:
The dataset includes the following global phonemes: [`exh`,`axh`,`vf`,`cl`,`mlem`,`hx`], `exh` and `axh` for unvoiced and voiced exhales, `vf` for vocal fry, `cl` for stops, `mlem` for mouth clicks, `hx` for unvoiced sounds (ie. the `h` sound in "white")

As of today (2026/03/03), the dataset's Mandarin Chinese section is complete

## Song List:
See [song list](/song_list)

# Credits:
Voice provided by Jonathan Huang 黃奕晨, owner of ArchiVoice, [X/Twitter](https://x.com/NekroTheCorpse)

# License:
<a href="https://github.com/Archivoice/ACV-002">ACV-002</a> © 2026 by <a href="https://github.com/Archivoice">YiChen Huang</a> is licensed under <a href="https://creativecommons.org/licenses/by-sa/4.0/">CC BY-SA 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">

The license only applies to direct use of the dataset and models mainly featuring the voice of ACV-002, and does not apply to models trained via parallel training.\
Models trained using ACV-002 as supplementary data can follow its own license.
