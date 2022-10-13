# handin assignments
Checkers(aka graders) are located here: https://github.com/jestarray/howtocode/tree/main/graders
Each folder is an assignment which is also reflected in `config.rktd`
## to place assignments in dirs here:
run `racket GEN_HANDIN_FOLDER.rkt` in pollen writeups

# NOTE: CLIENT MUST CONNECT USING  `https://` so `https:jestlearn.com:7979`

## to run the server
while in this directory
`nohup xvfb-run racket -l handin-server > /dev/null &`

## restarting the server
kill xvfb and racket

## for local testing copy from:
`(collection-path "handin-server")`
which is at(backup the production pem):
`cp ~/.racket/8.6/pkgs/handin/handin-server/private-key.pem ./`
and
`(collection-path "handin-server")`
which is at(backup the production pem):
`cp ~/.racket/8.6/pkgs/handin/handin-client/server-cert.pem ./`

## to reinstall handin under new config:
`raco setup handin-client`