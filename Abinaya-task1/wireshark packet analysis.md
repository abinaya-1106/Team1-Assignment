<h1>Part-B</h1>
<h2>1). Top 5 protocols</h2>
<p>IP - 89.2%</p>
<p>TCP - 70.3%</p>
<p>UDP - 18.9%</p>
<p>ARP - 10.8%</p>
<p>SSDP - 7.2%</p>
<p><b>Internet Protocol</b>:Each device on a network has a unique IP address.Internet protocol ensures each packet knows where it’s going (destination IP) and where it came from (source IP).IP packets travel independently and they may take different routes as well.Here data is broken into smaller packets and each packet has a source and destination address.</p>
<p><b>Transmission control protocol</b>:Each byte of data is numbered, and segments carry sequence numbers.It uses a sliding window to prevent the sender from overwhelming the receiver.At the server end TCP breaks down application data into smaller packets and at the reciever end it reassembles it back. The reciever sends an acknowledgement once all the data segements are recieved.</p>
<p><b>User datagram protocol</b>:Unlike TCP, there is no connection set up prior to sending the data. There is no acknowledgement recieved from the reciever. And if some data packets are lost during transmission, UDP does not care while TCP resends it again.But it is faster than TCP and functions similar to TCP in the aspect of transferring data packets.</p>
<p><b>Address Resolution protocol</b>:This is used to map IP address to MAC address.If the MAC address is not found in the ARP cache computer sends a ARP request and device with that particular IP replies and the computer stores its MAC address.</p>
<p><b>Simple Service discovery protocol</b>:It is used for discovering other devices on the same local network. Whenever a new device enters the network, it announces itself and devices who want to connect with them can connect.</p>
<h2>2). Query decumentation:</h2>
<h3>Query 1:</h3>
<p>Domain being queried - user-images.githubusercontent.com</p>
<p>DNS server IP - 10.20.1.21</p>
<p>Response IP address - 10.53.135.192</p>
<p>Response time - 0.037 s</p>
<h3>Query 2:</h3>
<p>Domain being queried - user-images.githubusercontent.com</p>
<p>DNS server IP - 10.20.1.21</p>
<p>Response IP address - 10.53.135.192</p>
<p>Response time - 0.036 s</p>
<h3>Query 3:</h3>
<p>Domain being queried - user-images.githubusercontent.com</p>
<p>DNS server IP - 10.20.1.21</p>
<p>Response IP address - 10.53.135.192</p>
<p>Response time - 0.034 s</p>
<h2>3).</h2>
<p>We need this handshake as it is like an agreement between server and client before data transfer.SYN is a request that the client sends to the server telling that it wants to send data starting with this particular sequence of numbers.Server responds to the client request with SYN-ACK signal bits set.Using SYN, client acknowledges the response of the server and they both establish a reliable connection with which they will start the actual data transfer.</p>
<h2>4). </h2>
<p>Yes, in http filter actual data can be seen as http does not encrypt data. The request url's and headers are visible. But after applying tls filter, only encrypted data is seen, i.e, the actual data is not seen.This is because https encypts data for saftey purposes. So anyone monitoring the network(here wireshark) cannot see the data. </p>

