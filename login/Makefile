all:
	# find ./ -name ".DS_Store" -depth -exec rm {} \;
	adm compile tpl --src=../login --package=login --var loginTmpl
	adm combine js --src=./assets/src/js/combine/ --dist=./assets/login/dist/all.min.js
	adm combine css --src=./assets/src/css/ --dist=./assets/login/dist/all.min.css
	adm compile asset --src=./assets/login/dist/ --dist=./ --package=login
	GO111MODULE=off go fmt ./...