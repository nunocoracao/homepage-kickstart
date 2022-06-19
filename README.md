# Homepage Kickstart

Install Docker

Install VS Code

Install VS Code Remote - Containers

Install git

Git Clone

VS Code open folder 
File > Open Folder

press + in remote extension

Open Current Folder in Container

wait for image to build

press + to open a new terminal

hugo new site . --force

git submodule add -b stable https://github.com/jpanther/congo.git themes/congo

mkdir config && mkdir config/_default

rm config.toml

cp themes/congo/config/_default/*.toml config/_default/

echo 'theme = "congo"' | cat - config/_default/config.toml > temp && mv temp config/_default/config.toml

git submodule update --remote --merge

hugo new posts/my-first-post.md

setup profile view

## config.toml
baseURL

## laanguage.en.toml
title
description
author stuff

## params.toml
layout to profile
enable search
colorscheme ocean
showAppearanceSwitcher

## articles
add categories and tags
explain draft tag

## run 
Hugo server -D
Hugo server
Hugo

## configure deploy
firebase stuff

firebase create project
firebase login
firebase init
firebase deploy
