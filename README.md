ddg-webtester
=============
The script tests the goodies and spice plugins which are part of Duckduckgo instant answers.


Dependencies
------------

The script requires:
 * String::Util
 * File::DirWalk
 * LWP
 * URI::Escape
 * JSON
 * LWP::Protocol::https

If you have working installation of perl run:
      
       sudo cpanm String::Util  File::DirWalk  LWP  URI::Escape  JSON  LWP::Protocol::https

to take care of all dependencies. 


Exampe Run
----------

perl webtester.pl ~/zeroclickinfo-goodies

DDG::Goodie::CurrencyIn
  currency in australia Test OK
  currency in AU Test OK

DDG::Goodie::Calculator
  $3.43+$34.45 Test OK
  64*343 Test OK

DDG::Goodie::SharkWeek
  shark week schedule Test FAIL
  shark week Test FAIL

DDG::Goodie::Unicornify

DDG::Goodie::CanadaPost
  canada post 123456789 Test FAIL

DDG::Goodie::RubiksCubePatterns
  rcube stripes Test OK
  rcube cube in a cube Test OK
  rcube swap centers Test OK

DDG::Goodie::Regexp
  regexp /(.*)/ ddg Test OK

DDG::Goodie::TimezoneConverter
  10:00AM MST to PST Test OK
  19:00 UTC to EST Test OK
  1am UTC to PST Test OK

DDG::Goodie::USPS
  EA 000 000 000 US Test FAIL
  usps 7000 0000 0000 0000 0000 Test OK

DDG::Goodie::Jira
  SOLR-4530 Test OK
  IdentityHtmlMapper solr-4530 Test OK

DDG::Goodie::UnixTime
  unix time 0000000000000 Test OK
  epoch 0 Test OK
  epoch 2147483647 Test OK

DDG::Goodie::Paper

DDG::Goodie::Base64
  base64 encode foo Test OK
  base64 decode dGhpcyB0ZXh0 Test OK

DDG::Goodie::HexToASCII
  ascii 0x74657374 Test OK
  ascii 0x5468697320697320612074657374 Test OK

DDG::Goodie::Braille

DDG::Goodie::VIN
  1g8gg35m1g7123101 Test OK
  vin 1g8gg35m1g7123101 Test OK
  1g8gg35m1g7123101 vehicle identification number Test OK
  1g8gg35m1g7123101 tracking Test OK

DDG::Goodie::Ascii
  0110100001100101011011000110110001101111 to ascii Test OK

DDG::Goodie::LaserShip
  LL12345678 Test OK

DDG::Goodie::ColorCodes
  hex color code for cyan Test OK
  rgb(173 Test OK
  216 Test FAIL
  230) Test FAIL
  hsl 194 0.53 0.79 Test OK
  cmyk(0.12 Test FAIL
  0 Test FAIL
  0 Test FAIL
  0) Test FAIL
  #00ff00 Test OK

DDG::Goodie::HTMLEntities
  &#33 Test OK
  html entity &amp Test OK

DDG::Goodie::IPS
  EM999999999IN Test OK

DDG::Goodie::Factors
  factors of 30 Test OK
  72 factors Test OK

DDG::Goodie::ZappBrannigan

DDG::Goodie::Morse
  morse ... --- ... Test OK
  morse SOS Test OK

DDG::Goodie::HelpLine
  suicide hotline Test FAIL

DDG::Goodie::CryptHashCheck

DDG::Goodie::DaysBetween
  days between 01/31/2000 01/31/2001 Test OK
  days between 01/31/2000 01/31/2001 inclusive Test OK

DDG::Goodie::Tips
  20% tip on $21.63 Test FAIL
  20 percent tip for a $20 bill Test FAIL

DDG::Goodie::Phonetic

DDG::Goodie::Fibonacci
  fib 7 Test OK
  fibonacci 33 Test OK

DDG::Goodie::ResistorColors
  4.7k ohm Test OK
  1Ω Test OK

DDG::Goodie::Coin

DDG::Goodie::RouterPasswords
  belkin f5d6130 default password Test FAIL
  alcatel office 4200 Test FAIL

DDG::Goodie::Rafl

DDG::Goodie::Xor
  4 xor 5 Test OK
  5 ⊕ 79 Test OK
  9489 xor 394 xor 9349 xor 39 xor 29 xor 4967 xor 3985 Test OK

DDG::Goodie::Poker
  poker odds three of a kind Test OK
  probability poker flush Test OK

DDG::Goodie::Hijri
  22/8/2003 to the hijri calendar Test OK
  23/6/1424 to gregorian Test OK

DDG::Goodie::Rot13

DDG::Goodie::PercentError
  percent-error 34.5 35 Test OK
  %err 41 43 Test OK
  %-error 2.88 2.82 Test OK

DDG::Goodie::Randagram
  randagram jazz hands Test FAIL

DDG::Goodie::LeetSpeak

DDG::Goodie::Frequency

DDG::Goodie::ReverseResistorColours
  red yellow white gold resistor Test OK
  resistor red yellow white Test OK

DDG::Goodie::Chars
  chars test Test OK
  chars this is a test Test OK

DDG::Goodie::Epoch
  epoch Test OK

DDG::Goodie::UnixPermissions
  chmod 755 Test OK
  permission 0644 Test OK

DDG::Goodie::GUID
  guid Test OK
  uuid Test OK

DDG::Goodie::JsKeycodes

DDG::Goodie::PrivateNetwork
  private networks Test OK
  private ips Test OK

DDG::Goodie::AspectRatio
  aspect ratio 4:3 640:? Test OK

DDG::Goodie::UPS
  1Z0884XV0399906189 Test OK
  ups 1Z0884XV0399906189 Test OK

DDG::Goodie::RandomName
  random name Test FAIL
  random person Test FAIL

DDG::Goodie::DateMath
  Jan 1 2012 plus 32 days Test OK
  1/1/2012 plus 5 months Test OK
  January first minus ten days Test OK

DDG::Goodie::PublicDNS
  public dns Test OK

DDG::Goodie::Capitalize
  capitalize this Test OK
  uppercase that Test OK

DDG::Goodie::Sha
  SHA this Test OK
  sha-512 that Test OK
  sha512sum dim-dims Test OK

DDG::Goodie::POTUS

DDG::Goodie::DuckDuckGo

DDG::Goodie::Sort
  sort -3 -10 56 10 Test FAIL
  sort descending 10 Test FAIL
  -1 Test FAIL
  +5.3 Test FAIL
  -95 Test FAIL
  1 Test FAIL

DDG::Goodie::Week
  what is the current week Test FAIL
  what was the 5th week of this year Test FAIL
  Network Error

DDG::Goodie::ISO639
  iso639 english Test OK
  iso639 ab Test OK

DDG::Goodie::Reverse
  reverse esrever Test OK

DDG::Goodie::FlipText
  flip my sentence Test OK
  mirror text Test OK

DDG::Goodie::Average
  average 12 Test OK
  45 Test FAIL
  78 Test FAIL
  1234 Test FAIL
  avg 1 Test FAIL
  2 Test FAIL
  3 Test FAIL
  root mean square 1 Test OK
  2 Test FAIL
  3 Test FAIL

DDG::Goodie::IDN

DDG::Goodie::ParseCron

DDG::Goodie::Dice
  throw dice Test OK
  roll 5 dice Test OK
  roll 3d12 Test OK

DDG::Goodie::Roman
  roman numeral MCCCXXXVII Test OK
  roman 1337 Test OK
  roman IV Test OK

DDG::Goodie::BirthStone
  birthstone april Test FAIL
  may birth stone Test FAIL

DDG::Goodie::Unicode
  U+590c Test OK
  unicode white smiling face Test OK

DDG::Goodie::PigLatin
  pig latin i love duckduckgo Test OK

DDG::Goodie::Unidecode
  unidecode møæp Test OK
  unidecode åäº° Test OK

DDG::Goodie::ABC
  choose yes or no Test OK
  choose heads or tails Test OK
  choose this or that or none Test OK

DDG::Goodie::DHL
  DHL 123456789 Test OK
  tracking 1234567891 Test OK

DDG::Goodie::UN
  UN Number 0009 Test OK

DDG::Goodie::Palindrome

DDG::Goodie::NLetterWords

DDG::Goodie::MoonPhases

DDG::Goodie::FedEx
  fedex 9241990100130206401644 Test OK
  federal express 9241990100130206401644 Test OK

DDG::Goodie::GoldenRatio
  golden ratio 900:? Test OK
  golden ratio ?:123.345 Test OK

DDG::Goodie::Anagram
  anagram of filter Test OK
  anagram filter 5 Test OK

DDG::Goodie::UnicodeFuzzySearch

DDG::Goodie::Passphrase

DDG::Goodie::Perimeter
  circumference circle 1 Test OK
  perimeter hexagon 45 Test OK
  perimeter of triangle 1.5 2 3.2 Test OK
  perimeter of rectangle 1 2 Test OK
  perimeter of square 3 Test OK

DDG::Goodie::Base
  255 in hex Test OK
  255 in base 16 Test OK
  42 in binary Test OK

DDG::Goodie::SigFigs
  sigfigs 01.1234000 Test OK
  significant figures 000123000 Test OK

DDG::Goodie::Chess960
  chess960 random Test OK

DDG::Goodie::AltCalendars
  heisei 24 Test FAIL
  meiji 1 Test FAIL

DDG::Goodie::HKDK
  CU123456789DK Test OK
  EE123456789HK Test OK

DDG::Goodie::EmToPx
  10 px to em Test OK
  12.2 px in em assuming a 12.2 font size Test OK

DDG::Goodie::Fortune
  unix fortune cookie Test OK

DDG::Goodie::Dewey
  dewey 644 Test OK
  etymology in the dewey decimal system Test OK
  dewey decimal system 640s Test OK
  dewey decimal system naturalism Test OK

DDG::Goodie::Atbash

DDG::Goodie::TitleCase
  titlecase test Test OK

DDG::Goodie::Binary
  foo in binary Test OK
  0x1e to binary Test OK
