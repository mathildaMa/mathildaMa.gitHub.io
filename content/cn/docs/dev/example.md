
---
title: "UML 示例"
weight: 10
---

## PlantUML 绘制 UML 图

直接在 .md 文件中书写:

    <div class="plantuml">
        @startuml
        Alice -> Bob: Authentication Request
        Bob --> Alice: Authentication Response

        Alice -> Bob: Another authentication Request
        Alice <-- Bob: another authentication Response
        @enduml
    </div>

运行如下:

<div class="plantuml">
    @startuml
    Alice -> Bob: Authentication Request
    Bob --> Alice: Authentication Response

    Alice -> Bob: Another authentication Request
    Alice <-- Bob: another authentication Response
    @enduml
</div>

如果你本地有 plantuml server, 可以在 config.toml 中配置本地  plantuml server 地址:

    [params]
    plantuml_url="http://www.plantuml.com/plantuml/svg/"


## mermaid 绘制 UML 图

直接在 .md 文件中书写:

    <div class="mermaid">
        sequenceDiagram
        Alice->>+John: Hello John, how are you?
        Alice->>+John: John, can you hear me?
        John-->>-Alice: Hi Alice, I can hear you!
        John-->>-Alice: I feel great!
    </div>

运行如下:

<div class="mermaid">
    sequenceDiagram
    Alice->>+John: Hello John, how are you?
    Alice->>+John: John, can you hear me?
    John-->>-Alice: Hi Alice, I can hear you!
    John-->>-Alice: I feel great!
</div>

