#nonStaticISF version

- Build on AAPS master

- Changes to default behaviour:

- profile ISF will be used as reference around the clock
- in the SMB Tab 3 bg points and factors have to be defined once
- also define max and min ISF allowed for safety reasons in SMB Tab
- then a formula will be derived from ISF@bg1-3 to calculate a curve for the current ISF
- 2 curves will be calculated. curve 1 for values between bg1 and bg1, curve2 for values between 
  bg2 and bg3
- This way you could have your profile isf between bg1 and bg2 and a different one above bg2
- ISF(bg)=m/bg+a, where m and a have been caluculated to match the given ISF@bg1, ISF@bg2 and 
  ISF@bg3;


This way the curve will vary over the day a bit if different ISF values are defined around the clock in profile;


I am not a professional programmer, this has to be used careful as a dev version!
Nevertheless i use this version for my son with good results so far

Reason to build this version was:

- unfortunately the dynamic ISF approach from TimS and ChrisW is not working well for my son
- the current bug in dev-i,
- and i wanted more control back and some kind of circadian behaviour back in ISF values





# AndroidAPS

* Check the wiki: https://androidaps.readthedocs.io
*  Everyone who’s been looping with AndroidAPS needs to fill out the form after 3 days of looping  https://docs.google.com/forms/d/14KcMjlINPMJHVt28MDRupa4sz4DDIooI4SrW0P3HSN8/viewform?c=0&w=1

[![Support Server](https://img.shields.io/discord/629952586895851530.svg?label=Discord&logo=Discord&colorB=7289da&style=for-the-badge)](https://discord.gg/4fQUWHZ4Mw)

[![Build status](https://travis-ci.org/nightscout/AndroidAPS.svg?branch=master)](https://travis-ci.org/nightscout/AndroidAPS)
[![Crowdin](https://d322cqt584bo4o.cloudfront.net/androidaps/localized.svg)](https://translations.androidaps.org/project/androidaps)
[![Documentation Status](https://readthedocs.org/projects/androidaps/badge/?version=latest)](https://androidaps.readthedocs.io/en/latest/?badge=latest)
[![codecov](https://codecov.io/gh/MilosKozak/AndroidAPS/branch/master/graph/badge.svg)](https://codecov.io/gh/MilosKozak/AndroidAPS)
dev: [![codecov](https://codecov.io/gh/MilosKozak/AndroidAPS/branch/dev/graph/badge.svg)](https://codecov.io/gh/MilosKozak/AndroidAPS)


![BTC](https://bitit.io/assets/coins/icon-btc-1e5a37bc0eb730ac83130d7aa859052bd4b53ac3f86f99966627801f7b0410be.svg) 3KawK8aQe48478s6fxJ8Ms6VTWkwjgr9f2
