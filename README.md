# Vietnamese Human Writing

A skill for writing and editing Vietnamese using 53 rules, seven revision passes, and 12 final acceptance checks. The instructions are bilingual; the complete Vietnamese rules remain unchanged.

"Human writing" describes natural, purposeful prose. This project does not classify authorship or promise to bypass AI detectors.

[Tiếng Việt](#tiếng-việt) · [Examples](skills/vietnamese-human-writing/references/examples.md) · [Complete rules](skills/vietnamese-human-writing/references/master-writing-rules.md)

## What it does

- Preserve facts, terminology, chronology, quotations, and the author's intention.
- Remove unsupported praise, clichés, empty conclusions, and mechanical sentence patterns.
- Adapt to prose, dialogue, journalism, analysis, history, science, and literary writing.
- Use rhythm statistics as editing signals when measurement is appropriate, with the source's original exceptions.

The skill requires no executable scripts or external service. It instructs the assistant to read the complete rules before editing. Its quality still depends on the model and the supplied source material.

## Install in Claude

1. Download the separate `vietnamese-human-writing.zip` distributed with this project, or ZIP the `skills/vietnamese-human-writing` folder yourself.
2. Keep `vietnamese-human-writing/` as the single top-level directory in the ZIP. Its `SKILL.md` must be directly inside it.
3. In Claude, enable **Settings → Capabilities → Code execution and file creation**, then open **Customize → Skills**.
4. Select **+ → Create skill → Upload a skill**, upload the ZIP, and enable the skill.

For managed accounts, available options depend on organization settings. Follow the [official installation guide](https://support.claude.com/en/articles/12512180-use-skills-in-claude) if the interface changes. Do not upload the repository ZIP as a skill.

## Try it

```text
Dùng Vietnamese Human Writing để viết lại đoạn sau theo Bộ quy tắc C.
Giữ nguyên số liệu, tên riêng và ý nghĩa. Chỉ trả đoạn đã sửa:
[dán văn bản]
```

```text
Use Vietnamese Human Writing to edit this Vietnamese dialogue for primary
school pupils. Keep the mathematical meaning and character voice.
Return only the dialogue:
[paste dialogue]
```

### Before

> Dự án thư viện lớp học không chỉ khẳng định vai trò then chốt của nhà trường mà còn mở ra một tương lai đầy hứa hẹn. Sau hai tuần, học sinh góp được 120 quyển sách.

### After

> Sau hai tuần, học sinh góp được 120 quyển sách cho thư viện lớp học.

This hypothetical example preserves the time and count while removing unsupported praise. It is an editorial illustration, not a measured model benchmark. See [more examples](skills/vietnamese-human-writing/references/examples.md).

## Repository contents

| Path | Purpose |
| --- | --- |
| `skills/vietnamese-human-writing/SKILL.md` | Bilingual instructions and activation description |
| `skills/vietnamese-human-writing/references/master-writing-rules.md` | Unchanged Vietnamese source, R01–R53 and sections I–XII |
| `skills/vietnamese-human-writing/references/examples.md` | Four before/after examples |
| `skills/vietnamese-human-writing/agents/openai.yaml` | Optional metadata for compatible Codex interfaces |
| `tests/scenarios.md` | Manual evaluation prompts and acceptance criteria |
| `LICENSE` | MIT license |

## Publish on GitHub

1. Create a public repository named `vietnamese-human-writing`.
2. Extract the repository ZIP and upload the contents of its top-level folder: `README.md`, `LICENSE`, `skills/`, and `tests/`.
3. In **About → Edit repository metadata → Topics**, add:
   `claude-skills`, `agent-skills`, `vietnamese`, `writing`, `editing`.
4. Optionally create a GitHub release and attach the separate installation ZIP.

Suggested repository description:

> Write and edit natural Vietnamese with Bộ quy tắc C: 53 rules, seven revision passes, and bilingual instructions.

Topics help people discover the repository. This does not constitute endorsement by Anthropic, and stars are added by GitHub users. See [GitHub's topic guide](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics).

## Evaluation and contributions

Use [the manual scenarios](tests/scenarios.md) on the actual target model after installation. Record the model, date, prompt, and raw output when reporting a problem. Structural validation alone does not establish editing quality or confirm installation in Claude.

The Vietnamese reference is the authoritative source. Propose changes explicitly rather than silently weakening a rule. Submit minimal examples with no private information.

## Tiếng Việt

Skill này dùng để viết mới, viết lại và biên tập tiếng Việt. Bản gốc giữ nguyên đủ 53 quy tắc, 7 vòng kiểm tra và 12 điều kiện chấp nhận. Hướng dẫn sử dụng có cả tiếng Anh và tiếng Việt.

Tên "Human Writing" chỉ mục tiêu viết tự nhiên, rõ nghĩa và có giọng riêng. Bộ quy tắc không xác định chắc chắn tác giả là người hay AI, cũng không bảo đảm vượt qua công cụ phát hiện AI.

### Cài vào Claude

Tải `vietnamese-human-writing.zip`, vào **Customize → Skills → + → Create skill → Upload a skill**, tải ZIP lên rồi bật skill. Bật **Code execution and file creation** trong **Settings → Capabilities** nếu cần. Dùng ZIP cài đặt riêng, không dùng ZIP chứa toàn bộ repository.

### Đưa lên GitHub

Tạo repository công khai tên `vietnamese-human-writing`. Giải nén gói repository rồi đưa `README.md`, `LICENSE`, `skills/` và `tests/` lên thư mục gốc. Thêm topic `claude-skills` trong phần **About**. Có thể đính kèm ZIP cài đặt vào một GitHub Release để người khác tải dễ hơn.

### Cách yêu cầu

```text
Áp dụng Vietnamese Human Writing và Bộ quy tắc C cho văn bản dưới đây.
Giữ nguyên dữ kiện, thuật ngữ và giọng người viết.
Chỉ trả văn bản cuối theo định dạng ban đầu.
[dán văn bản]
```

Nếu cần báo cáo, yêu cầu riêng: "Nêu lỗi dữ kiện, lỗi văn phong và lý do sửa." Chỉ yêu cầu thống kê khi văn bản và cách tính phù hợp.

### Giấy phép

Dự án dùng MIT: cho phép sử dụng, sửa và phân phối với điều kiện giữ thông báo bản quyền và giấy phép. Xem [LICENSE](LICENSE).

## References

- [Create custom skills — Claude Help Center](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills)
- [Use skills in Claude — Claude Help Center](https://support.claude.com/en/articles/12512180-use-skills-in-claude)
- [Repository topics — GitHub Docs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics)
- [Stars — GitHub Docs](https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars)

Installation and publishing instructions checked against official documentation on 2026-10-11.

