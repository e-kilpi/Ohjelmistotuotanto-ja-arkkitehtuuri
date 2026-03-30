# Domain Model – RoomLight
### ASCII diagram

```
[LightingProfile] -------- applied to --------> [Room]
        |                                         |
        |                                         |
        |                                    has (1..n)
        |                                         |
        |                                         v
        |                                      [Device]
        |
        |
        v
     (1..n Rooms)

### Attributes

**LightingProfile:**
- name
- brightness

**Room:**
- room_id
- active_profile
- online/offline

**Device:**
- device_id
- on/off