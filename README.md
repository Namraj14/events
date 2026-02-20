# events

event
│
├── type
│     → What event happened
│     → Example: "click", "change", "input", "save"
│
├── target
│     → The actual element that triggered the event
│
│     ├── value
│     │     → Used for text inputs, combobox, textarea
│     │     → event.target.value
│
│     ├── name
│     │     → Used to identify which field triggered
│     │     → event.target.name
│
│     ├── checked
│     │     → Used for checkbox (true/false)
│     │     → event.target.checked
│
│     ├── dataset
│     │     → Used for custom HTML data-* attributes
│     │
│     │     ├── id
│     │     │     → If button has data-id="001xx"
│     │     │     → event.target.dataset.id
│     │
│     │     ├── account
│     │     │     → If button has data-account="001xx"
│     │     │     → event.target.dataset.account
│     │
│     │     └── anyOtherCustomData
│
│     ├── label
│     │     → Button label (rarely used)
│
│     └── other DOM properties
│
├── currentTarget
│     → Where event handler is attached
│     → Mostly same as target in simple LWC
│
├── detail
│     → ONLY for CustomEvent (child → parent communication)
│
│     ├── recordId
│     │     → event.detail.recordId
│
│     ├── name
│     │     → event.detail.name
│
│     ├── age
│     │     → event.detail.age
│
│     └── any custom object you send
│
├── bubbles
│     → Whether event propagates upward
│
├── composed
│     → Whether event crosses shadow DOM boundary
│
└── other internal browser properties
