# selfhosted-music-overview

selfhosted-music-overview intends to provide an overview of self-hostable music streaming servers and clients.

## Table of Contents

1. [Server Overview](#server-overview)
2. [Client Overview](#client-overview)
3. [Emoji Definitions](#emoji-definitions)
4. [How to Contribute](#how-to-contribute)
5. [Footnotes](#footnotes)


## Server Overview



|                                                              |                  Scrobbling                  |       Jukebox Mode       |     Read Tags      |     Write Tags     |                             API                              |              Share Music               |                  Multi-User                   |            Multi-Library             |                 Smart Playlists                 |  Heart/ Favorites  |   5 Star Rating    |    Replay Gain     |     Transcode      |                  free                  |                Demo                 |                    Source Code                     |                         License                         | Reviewed Version |                                                              |
| ------------------------------------------------------------ | :------------------------------------------: | :----------------------: | :----------------: | :----------------: | :----------------------------------------------------------: | :------------------------------------: | :-------------------------------------------: | :----------------------------------: | :---------------------------------------------: | :----------------: | :----------------: | :----------------: | :----------------: | :------------------------------------: | :---------------------------------: | :------------------------------------------------: | :-----------------------------------------------------: | :--------------: | ------------------------------------------------------------ |
|                                                              |                                              |                          |                    |                    |                                                              |                                        |                                               |                                      |                                                 |                    |                    |                    |                    |                                        |                                     |                                                    |                                                         |                  |                                                              |
| [Airsonic](https://airsonic.github.io/)                      |              :heavy_check_mark:              |                          |                    |                    |                           subsonic                           |                                        |              :heavy_check_mark:               |                                      |                                                 | :heavy_check_mark: |                    |                    | :heavy_check_mark: | :heavy_check_mark: :heavy_dollar_sign: |                 :x:                 |       [GitHub](https://airsonic.github.io/)        |  [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)  |                  | [Airsonic](https://airsonic.github.io/)                      |
| [Ampache](https://ampache.org/)                              |                                              |                          | :heavy_check_mark: | :heavy_check_mark: |                           subsonic                           |                                        |              :heavy_check_mark:               |                                      |               :heavy_check_mark:                | :heavy_check_mark: | :heavy_check_mark: |                    | :heavy_check_mark: |           :heavy_check_mark:           |  :heavy_check_mark: [^ampachedemo]  |   [GitHub](https://github.com/ampache/ampache/)    | [aGPLv3](https://www.gnu.org/licenses/agpl-3.0.en.html) |      5.1.0       | [Ampache](https://ampache.org/)                              |
| [Jellyfin](https://jellyfin.org/)                            | :heavy_check_mark: [^github-lastfm-jellyfin] |           :x:            | :heavy_check_mark: | :heavy_check_mark: |             jellyfin, subsonic[^addon-jellysub]              |           :heavy_check_mark:           |              :heavy_check_mark:               |          :heavy_check_mark:          |               :heavy_check_mark:                | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |           :heavy_check_mark:           | :heavy_check_mark: [^jellyfindemo]  |   [GitHub](https://github.com/jellyfin/jellyfin)   |  [GPLv2](https://www.gnu.de/documents/gpl-2.0.de.html)  |      10.7.7      | [Jellyfin](https://jellyfin.org/)                            |
| [Funkwhale](https://funkwhale.audio/)                        |                                              |                          |                    |                    | [WIP custom](https://docs.funkwhale.audio/api.html), [subsonic](https://docs.funkwhale.audio/developers/subsonic.html) |           :heavy_check_mark:           |                                               |                                      |                                                 |                    |                    |                    |                    |           :heavy_check_mark:           |                 :x:                 |  [GitLab](https://dev.funkwhale.audio/funkwhale)   |                     :grey_question:                     |                  | [Funkwhale](https://funkwhale.audio/)                        |
| [Lightweight Music Server](https://github.com/epoupon/lms)   |              :heavy_check_mark:              |                          | :heavy_check_mark: | :heavy_check_mark: |                       :grey_question:                        |                                        |              :heavy_check_mark:               |                                      |               :heavy_check_mark:                | :heavy_check_mark: |                    |                    |                    |           :heavy_check_mark:           |    :heavy_check_mark: [^lmsdemo]    |      [GitHub](https://github.com/epoupon/lms)      |  [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)  |                  | [Lightweight Music Server](https://github.com/epoupon/lms)   |
| [Logitech Media Server](https://www.mysqueezebox.com/download) |              :heavy_check_mark:              |     :grey_question:      | :heavy_check_mark: |        :x:         |                       :grey_question:                        |  :heavy_check_mark: [^logitech-share]  | :heavy_check_mark: :grey_question: [^review1] | :heavy_check_mark: [^logitech-multi] | :heavy_check_mark: [^logitech-comment-playlist] | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |           :heavy_check_mark:           |         :heavy_check_mark:          |  [GitHub](https://github.com/Logitech/slimserver)  |  [GPLv2](https://www.gnu.de/documents/gpl-2.0.de.html)  |       8.2        | [Logitech Media Server](https://www.mysqueezebox.com/download) |
| [mStream](https://mstream.io/)                               |                                              |                          |                    |                    |                       :grey_question:                        |           :heavy_check_mark:           |                                               |                                      |                       :x:                       |                    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |           :heavy_check_mark:           | :heavy_check_mark: [^demo-mstream]  | [GitHub](https://github.com/IrosTheBeggar/mStream) |  [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)  |                  | [mStream](https://mstream.io/)                               |
| [Navidrome](https://github.com/navidrome/navidrome)          |              :heavy_check_mark:              | :x: [^roadmap-navidrome] | :heavy_check_mark: |        :x:         |                           subsonic                           |        :x: [^roadmap-navidrome]        |              :heavy_check_mark:               |                 :x:                  |               :heavy_check_mark:                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |           :heavy_check_mark:           | :heavy_check_mark: [^navidromedemo] |  [GitHub](https://github.com/navidrome/navidrome)  |  [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html)  |      0.46.0      | [Navidrome](https://github.com/navidrome/navidrome)          |
| [Plex](https://www.plex.tv/)                                 |                                              |                          | :heavy_check_mark: | :heavy_check_mark: |                       :grey_question:                        | :heavy_check_mark: :heavy_dollar_sign: |              :heavy_check_mark:               |          :heavy_check_mark:          |               :heavy_check_mark:                | :heavy_check_mark: |                    |                    |                    |           :heavy_check_mark:           |   :heavy_check_mark: [^plexdemo]    |        [GitHub](https://github.com/plexinc)        |                     :grey_question:                     |                  | [Plex](https://www.plex.tv/)                                 |
| [Polaris](https://github.com/agersant/polaris)               |              :heavy_check_mark:              |     :grey_question:      | :heavy_check_mark: |        :x:         |                            custom                            |            :grey_question:             |              :heavy_check_mark:               |          :heavy_check_mark:          |               :heavy_check_mark:                | :heavy_check_mark: |                    |                    |                    |           :heavy_check_mark:           |                 :x:                 |   [GitHub](https://github.com/agersant/polaris)    |             [MIT](https://mit-license.org/)             |      0.13.5      | [Polaris](https://github.com/agersant/polaris)               |

[^github-mstream]: https://github.com/IrosTheBeggar/mStream
[^demo-mstream]: https://demo.mstream.io/
[^demo-subsonic]: http://demo.subsonic.org/login.view?user=guest2&password=guest
[^website-mpd]: http://www.musicpd.org/
[^github-mpd]: https://github.com/MusicPlayerDaemon/MPD
[^github-mopidy]: https://github.com/mopidy
[^github-koel]: https://github.com/koel/koel
[^website-emby]: https://emby.media/
[^github-ampache]: https://github.com/ampache/ampache/
[^plexdemo]: [Plex Demo](https://app.plex.tv/desktop/#!/)
[^jellyfindemo]: [Jellyfin Demo](https://demo.jellyfin.org/)
[^navidromedemo]: [Navidrome Demo](https://www.navidrome.org/demo/)
[^lmsdemo]: [lms Demo](https://lms.demo.poupon.io/)
[^ampachedemo]: [Ampache Demo](https://ampache.org/demo.html)


[^github-plex]: https://github.com/plexinc
[^github-emby]: https://github.com/MediaBrowser/Emby
[^github-jellyfin]: https://github.com/jellyfin/jellyfin
[^github-navidrome]: https://github.com/navidrome/navidrome
[^github-airsonic]: https://airsonic.github.io/
[^github-subsonic]: https://github.com/subsonic
[^gitlab-funkwhale]: https://dev.funkwhale.audio/funkwhale
[^github-lms]: https://github.com/epoupon/lms

[^website-funkwhale]: https://funkwhale.audio/
[^website-mstream]: https://mstream.io/
[^website-ampache]: https://ampache.org/
[^website-mopidy]: https://docs.mopidy.com/
[^website-koel]: https://koel.dev/
[^website-musicpd]: https://www.musicpd.org/
[^website-serviio]: https://www.serviio.org/
[^website-squeezebox]: https://www.mysqueezebox.com/download

[^website-jellyfin]: https://jellyfin.org

[^logitech-share]: [Native Plugin](https://github.com/Logitech/slimserver/tree/public/8.3/Slim/Plugin/UPnP) enabling UPnP/DNLA support
[^review1]: needs review
[^logitech-multi]: [Plugin](https://wiki.slimdevices.com/index.php/Multi_Library_plugin.html)
[^logitech-comment-playlist]: works best if music library has been analysed by MusicIP beforehand, otherwise limited capability
[^github-logitech]: https://github.com/Logitech/slimserver
[^github-lastfm-jellyfin]: https://github.com/jesseward/jellyfin-plugin-lastfm
[^roadmap-navidrome]: on navidrome''s public road map

[^addon-jellysub]: https://github.com/nvllsvm/jellysub



## Client Overview

|                                                              |      OS      |  Gapless Playback  |     Album View     |     Songs View     |    Folder View     |    Artist View     |     Genre View     |    Decade View     |     Year View      |  Playlist Support  |  Most Played Song  | Most Played Album  | Recently Played Song | Recently Played Album | Recently Added Song | Recently Added Album | Frequently Played Album |     Offline Mode     |              Download Music               |      Podcasts      |     Scrobbling     |              Musicbrainz               |   Similar Songs    |  Artist Top Songs  |    Shuffle Play    |    Random Album    | Favorites / Starred / Bookmark |      5 Stars       |  Search function   | Chromecast Support |  Android Auto   |     Dark Mode      |     Themeable      |    Open Source     |        free        | Smart Recommendations |   Video Support    |   Internet Radio   |                 API                 |                           f-droid                            |                     Source Code                     |                        License                        | Reviewed Version |                                                             |
| ------------------------------------------------------------ | :----------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------: | :------------------: | :-------------------: | :-----------------: | :------------------: | :---------------------: | :------------------: | :---------------------------------------: | :----------------: | :----------------: | :------------------------------------: | :----------------: | :----------------: | :----------------: | :----------------: | :----------------------------: | :----------------: | :----------------: | :----------------: | :-------------: | :----------------: | :----------------: | :----------------: | :----------------: | :-------------------: | :----------------: | :----------------: | :---------------------------------: | :----------------------------------------------------------: | :-------------------------------------------------: | :---------------------------------------------------: | :--------------: | ----------------------------------------------------------- |
|                                                              |              |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                      |                       |                     |                      |                         |                      |                                           |                    |                    |                                        |                    |                    |                    |                    |                                |                    |                    |                    |                 |                    |                    |                    |                    |                       |                    |                    |                                     |                                                              |                                                     |                                                       |                  |                                                             |
| [Dsub](https://github.com/daneren2005/Subsonic)              |   Android    | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          | :heavy_check_mark:  |         :x:          |           :x:           |  :heavy_check_mark:  |            :heavy_check_mark:             | :heavy_check_mark: |        :x:         |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |       :heavy_check_mark:       | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :grey_question: |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |          :x:          | :heavy_check_mark: | :heavy_check_mark: |              subsonic               |              :heavy_check_mark: [^fdroid-dsub]               |  [GitHub](https://github.com/daneren2005/Subsonic)  | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      5.5.2       | Dsub                                                        |
| [Finamp](https://github.com/UnicornsOnLSD/finamp)            | Android, iOS |  :grey_question:   | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          |         :x:         |         :x:          |           :x:           |  :heavy_check_mark:  |            :heavy_check_mark:             |        :x:         |        :x:         |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |       :heavy_check_mark:       |        :x:         | :heavy_check_mark: |        :x:         |       :x:       | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         |              Jellyfin               | :heavy_check_mark: [Link](https://f-droid.org/packages/com.unicornsonlsd.finamp/) |  [Github](https://github.com/UnicornsOnLSD/finamp)  |   [MPL 2.0](https://www.mozilla.org/en-US/MPL/2.0/)   |      0.5.1       | [Finamp](https://github.com/UnicornsOnLSD/finamp)           |
| [Gelli](https://github.com/dkanada/gelli)                    |   Android    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          | :heavy_check_mark:  |  :heavy_check_mark:  |           :x:           |         :x:          |                    :x:                    |        :x:         | :heavy_check_mark: |                  :x:                   | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |       :heavy_check_mark:       |        :x:         | :heavy_check_mark: |        :x:         |       :x:       | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |    :grey_question:    |        :x:         |        :x:         |              jellyfin               |              :heavy_check_mark: [^fdroid-gelii]              |     [GitHub](https://github.com/dkanada/gelli)      | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      1.3.2       | Gelli                                                       |
| [Polaris Android](https://github.com/agersant/polaris)       |   Android    |        :x:         |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          |         :x:         |  :heavy_check_mark:  |           :x:           |  :heavy_check_mark:  |                    :x:                    |        :x:         | :heavy_check_mark: |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |              :x:               |        :x:         | :heavy_check_mark: |        :x:         | :grey_question: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         |               custom                |             :heavy_check_mark: [^fdroid-polaris]             |    [GitHub](https://github.com/agersant/polaris)    |            [MIT](https://mit-license.org/)            |      0.13.5      | Polaris Android                                             |
| [substreamer](https://substreamerapp.com/)                   |   Android    |        :x:         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          |         :x:         |         :x:          |           :x:           |  :heavy_check_mark:  |            :heavy_check_mark:             | :heavy_check_mark: | :heavy_check_mark: |                  :x:                   | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |        :x:         |       :heavy_check_mark:       |        :x:         | :heavy_check_mark: | :heavy_check_mark: | :grey_question: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |  :heavy_check_mark:   |        :x:         |        :x:         |              subsonic               |                             :x:                              |                         :x:                         |                    :grey_question:                    |      0.5.1       | substreamer                                                 |
| [Subtracks](https://github.com/austinried/subtracks)         |   Android    | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |  :heavy_check_mark:   |         :x:         |         :x:          |   :heavy_check_mark:    |         :x:          | :grey_question:[^help-subtracks-download] |        :x:         | :heavy_check_mark: |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |       :heavy_check_mark:       |        :x:         | :heavy_check_mark: |        :x:         |       :x:       |   :white_circle:   |        :x:         | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         |              subsonic               |            :heavy_check_mark: [^fdroid-subtracks]            |  [GitHub](https://github.com/austinried/subtracks)  | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      1.0.1       | Subtracks                                                   |
| [Ultrasonic](https://www.f-droid.org/en/packages/org.moire.ultrasonic/) |   Android    |  :grey_question:   | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: |         :x:          |  :heavy_check_mark:   |         :x:         |  :heavy_check_mark:  |           :x:           |         :x:          |            :heavy_check_mark:             | :heavy_check_mark: | :heavy_check_mark: |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |       :heavy_check_mark:       | :heavy_check_mark: | :heavy_check_mark: |        :x:         |       :x:       | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |          :x:          | :heavy_check_mark: |        :x:         |              subsonic               |           :heavy_check_mark: [^fdroid-ultrasonic]            |       [GitHub](https://github.com/ultrasonic)       | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      2.23.1      | Ultrasonic                                                  |
| [Navidrome](https://github.com/navidrome/navidrome)          |     Web      |  :grey_question:   | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |  :heavy_check_mark:  |  :heavy_check_mark:   | :heavy_check_mark:  |  :heavy_check_mark:  |                         |         :x:          |            :heavy_check_mark:             |        :x:         | :heavy_check_mark: | :heavy_check_mark:[^cannot-write-tags] |        :x:         |        :x:         | :heavy_check_mark: |                    |       :heavy_check_mark:       | :heavy_check_mark: | :heavy_check_mark: |                    |                 | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         |              subsonic               |                        :white_circle:                        |       [GitHub](https://github.com/navidrome)        | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      0.46.0      | Navidrome                                                   |
| [Polaris Web](https://github.com/agersant/polaris)           |     Web      |        :x:         |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          |         :x:         |  :heavy_check_mark:  |           :x:           |         :x:          |                    :x:                    |        :x:         | :heavy_check_mark: |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |              :x:               |        :x:         | :heavy_check_mark: |        :x:         | :white_circle:  | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         |               custom                |                        :white_circle:                        |    [GitHub](https://github.com/agersant/polaris)    |            [MIT](https://mit-license.org/)            |      0.13.5      | Polaris Web                                                 |
| [Tauon Music Box](https://github.com/Taiko2k/TauonMusicBox)  |    Linux     | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         |        :x:         |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         |         :x:          |          :x:          |         :x:         |         :x:          |           :x:           |         :x:          |                    :x:                    |        :x:         | :heavy_check_mark: |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |       :heavy_check_mark:       | :heavy_check_mark: | :heavy_check_mark: |        :x:         |       :x:       |        :x:         | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         | Jellyfin, Plex, Koel, Emby, Spotify |                        :white_circle:                        | [Github](https://github.com/Taiko2k/TauonMusicBox/) | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      6.8.2       | [Tauon Music Box](https://github.com/Taiko2k/TauonMusicBox) |
| [Jellyamp](https://github.com/m0ngr31/jellyamp)              |   L, W, M    |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |        :x:         |        :x:         |         :x:          |          :x:          |         :x:         |         :x:          |           :x:           |         :x:          |                    :x:                    |        :x:         |        :x:         |                  :x:                   | :heavy_check_mark: |        :x:         | :heavy_check_mark: |        :x:         |       :heavy_check_mark:       |        :x:         | :heavy_check_mark: |        :x:         |       :x:       |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |  :heavy_check_mark:   |        :x:         |        :x:         |              Jellyfin               |                        :white_circle:                        |    [Github](https://github.com/m0ngr31/jellyamp)    |            [MIT](https://mit-license.org/)            |      1.1.1       | [Jellyamp](https://github.com/m0ngr31/jellyamp)             |
| [Sonixd](https://github.com/jeffvli/sonixd)                  |   L, W, M    | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |        :x:         |        :x:         | :heavy_check_mark: |        :x:         | :heavy_check_mark: |         :x:          |  :heavy_check_mark:   |         :x:         |  :heavy_check_mark:  |           :x:           | :x:[^sonixd-offline] |            :heavy_check_mark:             |        :x:         |        :x:         |                  :x:                   |        :x:         |        :x:         | :heavy_check_mark: | :heavy_check_mark: |       :heavy_check_mark:       |        :x:         | :heavy_check_mark: |        :x:         |       :x:       | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |          :x:          |        :x:         |        :x:         |         Jellyfin, Subsonic          |                        :white_circle:                        |     [Github](https://github.com/jeffvli/sonixd)     | [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) |      0.8.5       | [Sonixd](https://github.com/jeffvli/sonixd)                 |
|                                                              |              |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                    |                      |                       |                     |                      |                         |                      |                                           |                    |                    |                                        |                    |                    |                    |                    |                                |                    |                    |                    |                 |                    |                    |                    |                    |                       |                    |                    |                                     |                                                              |                                                     |                                                       |                  |                                                             |
|                                                              |      OS      |  Gapless Playback  |     Album View     |     Songs View     |    Folder View     |    Artist View     |     Genre View     |    Decade View     |     Year View      |  Playlist Support  |  Most Played Song  | Most Played Album  | Recently Played Song | Recently Played Album | Recently Added Song | Recently Added Album | Frequently Played Album |     Offline Mode     |              Download Music               |      Podcasts      |     Scrobbling     |              Musicbrainz               |   Similar Songs    |  Artist Top Songs  |    Shuffle Play    |    Random Album    | Favorites / Starred / Bookmark |      5 Stars       |  Search function   | Chromecast Support |  Android Auto   |     Dark Mode      |     Themeable      |    Open Source     |        free        | Smart Recommendations |   Video Support    |   Internet Radio   |                 API                 |                           f-droid                            |                     Source Code                     |                        License                        | Reviewed Version |                                                             |

[^fdroid-gelii]: https://f-droid.org/en/packages/com.dkanada.gramophone/
[^github-gelli]: https://github.com/dkanada/gelli
[^fdroid-finamp]: https://f-droid.org/en/packages/com.unicornsonlsd.finamp/
[^github-finamp]: https://github.com/UnicornsOnLSD/finamp
[^fdroid-ultrasonic]: https://www.f-droid.org/en/packages/org.moire.ultrasonic/
[^github-finamp]: https://github.com/UnicornsOnLSD/finamp

[^github-ultrasonic]: https://github.com/ultrasonic
[^gplay-substreamer]: https://play.google.com/store/apps/details?id=com.ghenry22.substream2&hl=en&gl=US
[^gitlab-funkwhale]: https://dev.funkwhale.audio/funkwhale/funkwhale-android
[^fdroid-subtracks]: https://f-droid.org/en/packages/com.subtracks/
[^fdroid-polaris]: https://f-droid.org/en/packages/agersant.polaris/
[^github-subtracks]: https://github.com/austinried/subtracks
[^fdroid-dsub]: https://f-droid.org/en/packages/github.daneren2005.dsub/
[^github-dsub]: https://github.com/daneren2005/Subsonic
[^fdroid-audinaut]: https://f-droid.org/en/packages/net.nullsum.audinaut/
[^github-audinaut]: https://github.com/nvllsvm/Audinaut
[^fdroid-subsonic]: https://f-droid.org/en/packages/net.sourceforge.subsonic.androidapp/
[^sourceforge-subsonic]: https://sourceforge.net/projects/subsonic/
[^github-navidrome]: https://github.com/navidrome

[^help-subtracks-download]: There is a download button. It doesn't work for me.
[^website-subsonic]: http://www.subsonic.org/pages/index.jsp
[^website-funkwhale]: https://funkwhale.audio/
[^fdroid-funkwhale]: https://f-droid.org/en/packages/audio.funkwhale.ffa/

[^github-stretto]: https://github.com/benkaiser/stretto
[^website-subfire]: https://subfireplayer.net/
[^github-subplayer]: https://github.com/peguerosdc/subplayer

[^cannot-write-tags]: Can't write tags to file.

[^github-strawberry]: https://github.com/strawberrymusicplayer/strawberry
[^github-amperfy]: https://github.com/BLeeEZ/amperfy
[^github-isub]: https://github.com/einsteinx2/iSubMusicStreamer
[^github-stretto]: https://github.com/benkaiser/stretto
[^sonixd-offline]: [Is planned](https://github.com/jeffvli/sonixd/issues/10)

## Emoji Definitions

- :heavy_check_mark: means yes, it is supported
- :x: means no, it is not supported
- :heavy_dollar_sign: means the service/feature has a price `p` where `p>0`
- :grey_question: means help wanted, original author wasn't sure or couldn't judge the covered topic.
- :white_circle: means the feature doesn't apply to this service and cannot be evaluated.
- an empty cell is missing information. It is not intentionally left blank.

## How to Contribute (WIP)

- work in an editor that supports no forced line breaks, otherwise you can't read the raw markdown table. VSCodium, Atom and others are suitable for raw markdown editing.

- work in an editor that supports some sort of [WYSIWYG](https://en.wikipedia.org/wiki/WYSIWYG) like [Typora](https://typora.io/)  otherwise it is a real mess to fill a markdown table. Typora can clean the final raw markdown table as well.

- To add a service it is always good to take the current version of the table to match the columns. I'll try to merge all PRs in a timely manner.

- open issue or a PR

- matrix-room: #selfhosted-music-overview

## Footnotes
