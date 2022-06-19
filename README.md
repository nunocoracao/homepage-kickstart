# Homepage Kickstart

hugo new site mywebsite

git init
git submodule add -b stable https://github.com/jpanther/congo.git themes/congo


themes/congo/config/_default


mkdir config
mkdir congig/_default

rm config.toml

cp themes/congo/*.toml config/_default/

hugo mod get -u