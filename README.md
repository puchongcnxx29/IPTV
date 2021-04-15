Free TV
=======

This is an M3U playlist for free TV channels around the World.

To use it point your IPTV player to https://raw.githubusercontent.com/Free-TV/IPTV/master/playlist.m3u8.

Philosophy
==========

The main goals for this playlist are listed below.

**Quality over quantity**

The less channels we support the better. The less countries we support the better.

- All channels should work well.
- As much as possible channels should be in HD, not SD.
- Only one URL per channel (no +1, no alternate feeds, no regional declinations)

**Only free channels**

If a channel is normally only available via commercial subscriptions it has nothing to do in this playlist. If on the other hand it is provided for free to everybody in a particular country, then it should be in this playlist.

- No paid channels
- Only channels which are officially provided for free (via DVB-S, DVB-T, analog, etc..)

**Only mainstream channels**

This is a playlist for everybody.

- No adult channels
- No channels dedicated to any particular religion
- No channels dedicated to any particular political party
- No channels made for a country and funded by a different country

Format
======

The m3u8 playlist is generated from the .md files by the .py script.

Each .md file represesnts a group. The `<h1>` line is used as the group title.
  
Only channels which URL column starts with `[>]` are included in the playlist.

Channels which are not in HD are marked with an `Ⓢ`.

Channels which use GeoIP blocking are marked with a `Ⓖ`.

Issues
======

Only create issues for bugs and feature requests.

Do not create issues to add/edit or to remove channels. If you want to add/edit/remove channels, create a pull request directly.

Pull Requests
=============

**Only modify .md files**

If your Pull Request modifies channels, only modify .md files. Do not modify m3u8 files in your pull request.

**Adding a new Channel**

To add a new channel, make a Pull Request.

- In your Pull Request you need to provide information to show that the channel is free.
- Use imgur.com to host the channel logo and point to it.
- If you have a valid HD stream, add it and put `[>]` in front of it.
- If you don't have an stream for the channel, add `[x]()` in the url column and place your channel in the Invalid category.
- If you have a stream but it doesn't work well, put the channel in the Invalid category and put `[x]` in front of the url.

**Removing a Channel**

To remove a channel, make a Pull Request.

In your Pull Request you need to provide information to show that the channel is only available via a private paid subscription.

Note: Public taxes (whether national or regional, whether called TV License or not) do not constitute a private paid subscription.

If a stream is broken, simply move the channel to the invalid category and replace `[>]` with `[x]` in the url column.

Supported Countries
===================

- France: TNT channels (DVB-T) and a few satellite channels.
- Germany: DVB-T
- Italy: DVB-T
- Ireland: Saorview
- Spain: DVB-T
- UK: Freeview
- USA: DVB-S, Pluto TV
