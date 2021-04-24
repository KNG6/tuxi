# Tuxi

Tuxi is a simple bash script which scrape google search for getting instant answers of your question on your terminal.
(ceci est en fork pour les français voulant utiliser ce script)


[Watch this Video Please](https://www.youtube.com/watch?v=EtwWvMa8muU)
> Also checkout my youtube channel for more scripts like this

## Requirements
* [pup](https://github.com/ericchiang/pup) - CLI tool for processing HTML.
* Recode
* jq 

## Installation
First run these commands.
```bash
git clone https://github.com/bugswriter/tuxi.git
cd tuxi
cp tuxi $HOME/.local/bin/tuxi
```

## Usage

```bash
tuxi "is linux better than windows"
Linux is very well secure as it is easy to
detect bugs and fix whereas Windows has a huge user
base, so it becomes a target of hackers to attack
windows system. Linux runs faster even with older hardware whereas
windows are slower compared to Linux.
```
* Quotations are optional if you want to search with some special character.
* You can write question directly like `tuxi linus torvalds birthday`

## How this work?
It simply use google search results.
By using pup I scrape google search results and get cream information like answer of one word question or paragraph which google show on top.
Sometimes Google give multiple cream information like one word results and other information on right In that case It show result of the basis of priority.
I do scraping with `pup` and use some Unix tools like `awk` `sed` to do the magic.

## License
Do whatever you want. Just don't make money from this and If you do 70% is mine.
