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


# Homepage Kickstart

hugo new site mywebsite
hugo new site . --force

git init
git submodule add -b stable https://github.com/jpanther/congo.git themes/congo


themes/congo/config/_default


mkdir config && mkdir config/_default

rm config.toml

cp themes/congo/config/_default/*.toml config/_default/

echo 'theme = "congo"' >> config/_default/config.toml

touch config/_default/module.toml

echo '[[imports]]
path = "github.com/jpanther/congo/v2"' >> config/_default/module.toml

hugo mod get -u
