# Discord API Kullanım Kılavuzu

Bu proje, Discord kullanıcıları ve sunucuları hakkında bilgi almak için kullanılan bir API sağlayıcısını kullanarak kayıt sistemlerinizi geliştirmek için kullanılabilir.
## API Erişim Bilgileri
API'ye erişim sağlamak için aşağıdaki URL'leri ve anahtarları kullanabilirsiniz:

    Kullanıcı Bilgileri: https://api.approvalcyber.dev/api/discord/users/{id}
    Sunucu Bilgileri: https://api.approvalcyber.dev/api/discord/guilds/{id}

## API Anahtarı

Başlıkta belirtilen anahtar ile API'ye erişim sağlayabilirsiniz:

    x-api-key: luppux

## Kullanıcı Bilgileri

Aşağıda bir kullanıcıdan alınan örnek veri yapısını görebilirsiniz:

```json

{
  "_id": {
    "$oid": "66cefe610bf423d1e2c03d05"
  },
  "id": "1163111088389357608",
  "username": "example_user",
  "globalName": "example_name",
  "names": [
    {
      "guildID": "guild_id_1",
      "guildName": "Example Guild",
      "tag": "✫",
      "displayName": "example_display_name | null",
      "genderSymbol": "♂️",
      "Date": 1725883894368
    }
  ],
  "__v": 0,
  "avatarDecoration": {},
  "banner": "https://example.com/banner.webp",
  "avatar": "https://example.com/avatar.webp",
  "guilds": [
    {
      "guildID": "guild_id_1",
      "guildName": "Example Guild",
      "guildBanner": "https://example.com/guild_banner.webp",
      "guildIcon": "https://example.com/guild_icon.webp",
      "boostStatus": true,
      "roles": [
        {
          "id": "role_id_1",
          "name": "Role Name",
          "color": "#c3c3f3"
        }
      ],
      "permissions": [
        "VIEW_CHANNEL",
        "SEND_MESSAGES"
      ],
      "displayName": "example_display_name",
      "name": {
        "guildID": "guild_id_1",
        "guildName": "Example Guild",
        "tag": "✫",
        "displayName": "example_display_name | null",
        "genderSymbol": "♂️",
        "Date": 1725883894368
      },
      "isOwner": false,
      "joinedAt": {
        "$date": "2024-08-30T23:44:30.484Z"
      },
      "owner": {
        "id": "owner_id",
        "username": "owner_username",
        "displayName": "owner_display_name"
      }
    }
  ]
}
```
## Sunucu Bilgileri

Aşağıda bir sunucudan alınan örnek veri yapısını görebilirsiniz:
```json

{
  "_id": {
    "$oid": "66cde25e942a00fdee0eb16f"
  },
  "guildID": "server_id",
  "name": "Example Server",
  "icon": null,
  "ownerId": "owner_id",
  "memberCount": 29,
  "premiumTier": 0,
  "afkTimeout": 300,
  "preferredLocale": "en-US",
  "roles": [
    {
      "id": "role_id",
      "name": "@everyone",
      "color": 0,
      "position": 0,
      "permissions": [
        "VIEW_CHANNEL",
        "SEND_MESSAGES"
      ],
      "emoji": null,
      "memberCount": 6,
      "members": [
        "member_id_1",
        "member_id_2"
      ]
    }
  ],
  "channels": [
    {
      "id": "channel_id",
      "name": "General Chat",
      "type": "GUILD_TEXT",
      "position": 0,
      "parentId": null,
      "topic": null,
      "nsfw": false,
      "rateLimitPerUser": 0
    }
  ]
}
```
Kullanım

    API'ye Erişim: API'ye erişim sağlamak için uygun URL ve anahtar kullanılarak GET isteği gönderilmelidir.
    Veri Analizi: Gelen JSON yanıtları üzerinde gerekli veriler çıkarılabilir ve kayıt sistemleri için kullanılabilir.

Katkıda Bulunma

Katkıda bulunmak isterseniz, lütfen bir pull request gönderin ya da bu repo hakkında herhangi bir sorun bildirin.
