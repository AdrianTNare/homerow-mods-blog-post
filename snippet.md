```json
{
    "description": "Home row mods - cmd, opt, shift, ctrl",
    "manipulators": [
        {
            "from": {
                "key_code": "a",
                "modifiers": { "optional": ["any"] }
            },
            "to_delayed_action": {
                "to_if_canceled": [{ "key_code": "a" }],
                "to_if_invoked": [{ "key_code": "vk_none" }]
            },
            "to_if_alone": [
                {
                    "halt": true,
                    "key_code": "a"
                }
            ],
            "to_if_held_down": [
                {
                    "halt": true,
                    "key_code": "left_command"
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "s",
                "modifiers": { "optional": ["any"] }
            },
            "to_delayed_action": {
                "to_if_canceled": [{ "key_code": "s" }],
                "to_if_invoked": [{ "key_code": "vk_none" }]
            },
            "to_if_alone": [
                {
                    "halt": true,
                    "key_code": "s"
                }
            ],
            "to_if_held_down": [
                {
                    "halt": true,
                    "key_code": "left_option"
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "d",
                "modifiers": { "optional": ["any"] }
            },
            "to_delayed_action": {
                "to_if_canceled": [{ "key_code": "d" }],
                "to_if_invoked": [{ "key_code": "vk_none" }]
            },
            "to_if_alone": [
                {
                    "halt": true,
                    "key_code": "d"
                }
            ],
            "to_if_held_down": [
                {
                    "halt": true,
                    "key_code": "left_shift"
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "f",
                "modifiers": { "optional": ["any"] }
            },
            "to_delayed_action": {
                "to_if_canceled": [
                    {
                        "halt": true,
                        "key_code": "f"
                    }
                ],
                "to_if_invoked": [{ "key_code": "vk_none" }]
            },
            "to_if_alone": [
                {
                    "halt": true,
                    "key_code": "f"
                }
            ],
            "to_if_held_down": [
                {
                    "halt": true,
                    "key_code": "left_control"
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "a" },
                    { "key_code": "s" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_command",
                    "modifiers": ["left_option"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "a" },
                    { "key_code": "d" }
                ]
            },
            "to": [
                {
                    "key_code": "left_command",
                    "modifiers": ["left_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "a" },
                    { "key_code": "f" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_command",
                    "modifiers": ["left_control"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "f" },
                    { "key_code": "s" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_control",
                    "modifiers": ["left_option"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "f" },
                    { "key_code": "d" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_control",
                    "modifiers": ["left_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "a" },
                    { "key_code": "s" },
                    { "key_code": "d" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_command",
                    "modifiers": ["left_option", "left_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "a" },
                    { "key_code": "s" },
                    { "key_code": "f" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_command",
                    "modifiers": ["left_option", "left_control"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "f" },
                    { "key_code": "s" },
                    { "key_code": "d" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_control",
                    "modifiers": ["left_option", "left_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "a" },
                    { "key_code": "s" },
                    { "key_code": "d" },
                    { "key_code": "f" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "left_command",
                    "modifiers": ["left_option", "left_shift", "left_control"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "semicolon",
                "modifiers": { "optional": ["any"] }
            },
            "to_delayed_action": {
                "to_if_canceled": [{ "key_code": "semicolon" }],
                "to_if_invoked": [{ "key_code": "vk_none" }]
            },
            "to_if_alone": [
                {
                    "halt": true,
                    "key_code": "semicolon"
                }
            ],
            "to_if_held_down": [
                {
                    "halt": true,
                    "key_code": "right_command"
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "l",
                "modifiers": { "optional": ["any"] }
            },
            "to_delayed_action": {
                "to_if_canceled": [{ "key_code": "l" }],
                "to_if_invoked": [{ "key_code": "vk_none" }]
            },
            "to_if_alone": [
                {
                    "halt": true,
                    "key_code": "l"
                }
            ],
            "to_if_held_down": [
                {
                    "halt": true,
                    "key_code": "right_option"
                }
            ],
            "type": "basic"
        },
        {
            "conditions": [
                {
                    "name": "k-tapped",
                    "type": "variable_if",
                    "value": 1
                }
            ],
            "from": {
                "key_code": "k",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "key_code": "k",
                    "repeat": true
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "k",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "set_variable": {
                        "name": "k-tapped",
                        "value": 1
                    }
                }
            ],
            "to_delayed_action": {
                "to_if_canceled": [
                    {
                        "set_variable": {
                            "name": "k-tapped",
                            "value": 0
                        }
                    }
                ],
                "to_if_invoked": [
                    {
                        "set_variable": {
                            "name": "k-tapped",
                            "value": 0
                        }
                    }
                ]
            },
            "to_if_alone": [{ "key_code": "k" }],
            "to_if_held_down": [{ "key_code": "right_shift" }],
            "type": "basic"
        },
        {
            "conditions": [
                {
                    "name": "j-tapped",
                    "type": "variable_if",
                    "value": 1
                }
            ],
            "from": {
                "key_code": "j",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "key_code": "j",
                    "repeat": true
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "j",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "set_variable": {
                        "name": "j-tapped",
                        "value": 1
                    }
                }
            ],
            "to_delayed_action": {
                "to_if_canceled": [
                    {
                        "set_variable": {
                            "name": "j-tapped",
                            "value": 0
                        }
                    }
                ],
                "to_if_invoked": [
                    {
                        "set_variable": {
                            "name": "j-tapped",
                            "value": 0
                        }
                    }
                ]
            },
            "to_if_alone": [{ "key_code": "j" }],
            "to_if_held_down": [{ "key_code": "right_control" }],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "semicolon" },
                    { "key_code": "j" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_command",
                    "modifiers": ["right_control"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "semicolon" },
                    { "key_code": "k" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_command",
                    "modifiers": ["right_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "semicolon" },
                    { "key_code": "l" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_command",
                    "modifiers": ["right_option"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "j" },
                    { "key_code": "l" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_control",
                    "modifiers": ["right_option"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "j" },
                    { "key_code": "k" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_control",
                    "modifiers": ["right_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "semicolon" },
                    { "key_code": "j" },
                    { "key_code": "k" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_command",
                    "modifiers": ["right_control", "right_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "j" },
                    { "key_code": "l" },
                    { "key_code": "k" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_control",
                    "modifiers": ["right_option", "right_shift"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "semicolon" },
                    { "key_code": "j" },
                    { "key_code": "l" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_command",
                    "modifiers": ["right_control", "right_option"]
                }
            ],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "semicolon" },
                    { "key_code": "j" },
                    { "key_code": "k" },
                    { "key_code": "l" }
                ]
            },
            "to_if_held_down": [
                {
                    "key_code": "right_command",
                    "modifiers": ["right_control", "right_shift", "right_option"]
                }
            ],
            "type": "basic"
        }
    ]
}
```
