# myansible

PLAY [Network get info] *****************************************************************************

TASK [Gathering Facts] *****************************************************************************

ok: [CS01]
ok: [AS02]
ok: [CS02]
ok: [AS01]

TASK [Get cofig] *****************************************************************************
ok: [AS01]
ok: [CS02]
ok: [CS01]
ok: [AS02]

TASK [Display hostname] *****************************************************************************
ok: [CS01] => {
    "msg": [
        "The hostname is: CS01",
        "The model is: 9SM7787EK4T",
        [
            "172.20.1.51"
        ]
    ]
}
ok: [CS02] => {
    "msg": [
        "The hostname is: CS02",
        "The model is: 9TOO6H4LGMT",
        [
            "172.20.1.52"
        ]
    ]
}
ok: [AS01] => {
    "msg": [
        "The hostname is: AS01",
        "The model is: 9MHG7DGEQP8",
        [
            "172.20.1.53"
        ]
    ]
}
ok: [AS02] => {
    "msg": [
        "The hostname is: AS02",
        "The model is: 9AIB191ZZ0P",
        [
            "172.20.1.54"
        ]
    ]
}

TASK [Config hostname] *****************************************************************************

ok: [CS01]
ok: [AS01]
ok: [CS02]
ok: [AS02]

TASK [show run] *****************************************************************************
ok: [CS02]
ok: [CS01]
ok: [AS01]
ok: [AS02]

TASK [Save output to file] *****************************************************************************
changed: [CS02]
changed: [CS01]
changed: [AS02]
changed: [AS01]

PLAY RECAP *****************************************************************************
AS01                       : ok=6    changed=1    unreachable=0    failed=0
AS02                       : ok=6    changed=1    unreachable=0    failed=0
CS01                       : ok=6    changed=1    unreachable=0    failed=0
CS02                       : ok=6    changed=1    unreachable=0    failed=0
