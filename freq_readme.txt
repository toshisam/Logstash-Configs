#I use freq.py quite often to do frequency analysis on logs.  To do this you need to create a /opt/freq folder and then download freq.py to it.  Then you need #to download my frequency tables from the freq folder on this github page.

#Example:

mkdir /opt/freq
wget https://github.com/MarkBaggett/MarkBaggett/raw/master/freq/freq.py
chmod +x /opt/freq/freq.py

# USING GIT DATA
# The example below assumes you ran "git clone https://github.com/SMAPPER/Logstash-Configs" while in /etc/logstash. If you used "git clone" in a different # folder than exchange /etc/logstash with your folder.
cp -f /etc/logstash/Logstash-Configs/freq/* /opt/freq/

# MANUAL DOWNLOAD:
#Then download my frequency tables from github using the following:

cd /opt/freq
wget https://github.com/SMAPPER/Logstash-Configs/raw/master/freq/dns.freq
wget https://github.com/SMAPPER/Logstash-Configs/raw/master/freq/doc.freq
wget https://github.com/SMAPPER/Logstash-Configs/raw/master/freq/file.freq
wget https://github.com/SMAPPER/Logstash-Configs/raw/master/freq/pdf.freq
wget https://github.com/SMAPPER/Logstash-Configs/raw/master/freq/uri.freq
wget https://github.com/SMAPPER/Logstash-Configs/raw/master/freq/xls.freq