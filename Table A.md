
## A. Details of Nodes and Elements

### A.1 Algorithm Node Properties

| Property    | Data Type     | Length Limit | Description                        |
|-------------|---------------|--------------|------------------------------------|
| `uid`       | String        | –            | Unique identifier of the algorithm |
| `title`     | String        | –            | Algorithm name                     |
| `category`  | String        | –            | Algorithm category                 |
| `intro`     | String        | 500 chars    | Brief introduction                 |
| `principle` | String        | 1000 chars   | Core principle / rationale         |
| `cpx_time`  | String        | –            | Time complexity                    |
| `cpx_space` | String        | –            | Space complexity                   |
| `keywords`  | Array[String] | ≤ 10         | List of keywords                   |
| `aliases`   | Array[String] | ≤ 5          | Alternative names / aliases        |

---

### A.2 Chunk Node Properties

| Property    | Data Type    | Length Limit | Description                                              |
|-------------|--------------|--------------|----------------------------------------------------------|
| `id`        | String       | –            | Unique chunk identifier (format: `{uid}_chunk_{index}`)  |
| `content`   | String       | 500 chars    | Cleaned text content                                     |
| `embedding` | Array[Float] | 1024 dims    | L2-normalized vector embedding                           |

---

### A.3 Example Node Properties

| Property     | Data Type | Length Limit | Description                                                 |
|--------------|-----------|--------------|-------------------------------------------------------------|
| `id`         | String    | –            | Unique example identifier (format: `{uid}_example_{index}`) |
| `title`      | String    | –            | Example title                                               |
| `description`| String    | –            | Example description                                         |
| `code`       | String    | 2000 chars   | Example code                                                |
| `solution`   | String    | –            | Explanation of the solution                                 |
| `lang`       | String    | –            | Programming language (default: `cpp`)                       |
| `has_code`   | Boolean   | –            | Whether the example includes code                           |

---

### A.4 Concept Node Properties

| Property | Data Type | Description                       |
|----------|-----------|-----------------------------------|
| `name`   | String    | Concept name (whitespace-trimmed) |

---