# Homepage Kickstart

hugo new site . --force

git submodule add -b stable https://github.com/jpanther/congo.git themes/congo

mkdir config && mkdir config/_default

rm config.toml

cp themes/congo/config/_default/*.toml config/_default/

echo 'theme = "congo"' | cat - config/_default/config.toml > temp && mv temp config/_default/config.toml

git submodule update --remote --merge

hugo new posts/my-first-post.md

setup profile view
