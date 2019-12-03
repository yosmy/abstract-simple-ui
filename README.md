# Compile

cd test

docker-compose \
-f docker/all.yml \
-p mobile_ui \
stop

cd ..

mv test/src ./

npm

rm -rf build/* && node_modules/.bin/babel src --copy-files --out-dir build
