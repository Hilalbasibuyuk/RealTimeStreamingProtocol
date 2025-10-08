# Real Time Streaming Protocol (RTSP)

Gerçek Zamanlı Akış Protokolü (RTSP), verileri aktaran sunucuyla doğrudan iletişim kurarak gerçek zamanlı verileri multimedyadan bir uç nokta cihazına aktaran uygulama düzeyinde bir ağ iletişim sistemidir. Ama ben önce RTSP değil RTP'ye değineceğim. Videolarımızı gerçek zamanlı olarak işleyen protokol RTP'dir. Bu gerçek zamanlı işlemin description(tanımını), play/pause gibi komutlarla tanımlamasını sağlayan şey RTSP'dir. RTSP bir aracıdır burada. Asıl "taşıma işi" RTP gibi bir protokol tarafından yapılır. Bu ikili (RTSP + RTP) birlikte çalışarak gerçek zamanlı akışı mümkün kılar.

### Özetle RTSP: "Ne oynatacağını, ne zaman başlayıp duracağını" söyler. Ama videonun kendisini taşımaz. RTSP bir kontrol protokolüdür diyebiliriz. 



## RTSP Commands

- **Options:** This request determines what other types of requests the media server will accept.
- **Describe:** A describe request identifies the URL and type of data.
- **Announce:** The announce method describes the presentation when sent from the client to the server and updates the description when sent from server to client.
- **Setup:** Setup requests specify how a media stream must be transported before a play request is sent.
- **Play:** A play request starts the media transmission by telling the server to start sending the data.
- **Pause:** Pause requests temporarily halt the stream delivery.
- **Record:** A record request initiates a media recording.
- **Teardown:** This request terminates the session entirely and stops all media streams.
- **Redirect:** Redirect requests inform the client that it must connect to another server by providing a new URL for the client to issue requests to.




# KAYNAKÇA
- https://www.wowza.com/blog/rtsp-the-real-time-streaming-protocol-explained
