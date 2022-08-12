sudo apt-get install build-essential libssl-dev git
cd /usr/local/src && sudo git clone https://github.com/wg/wrk.git && cd wrk
sudo make
sudo cp -r wrk /usr/local/bin
sudo apt install graphviz

https://linux-notes.org/ustanovka-wrk-v-unix-linux/

wrk 'http://localhost:9000/users/b29f95a2-499a-4079-97f5-ff55c3854fcb/articles'
go tool pprof http://localhost:9000/debug/pprof/profile?seconds=10