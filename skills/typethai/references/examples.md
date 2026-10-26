# Type Thai: examples

Bad → better examples for the rules in `../SKILL.md`. Section names match the **Check** list there. The "better" lines are candidates, not a verified phrasebook. Learn the pattern; don't copy the phrase.

## Phrases you can't vouch for

Invented colloquialisms, rejected by a native speaker:

| Invented | Built from | Plainer candidates (let the user judge) |
|---|---|---|
| เทสฟ้อง | "the test complains"; ฟ้อง = tattle/sue | เทสไม่ผ่าน, เทส fail |
| sync จะทับกลับ | "overwrite back" | sync รอบหน้าก็โดนทับอยู่ดี |
| ลองย้อน fix กลับ | "revert the fix back"; ย้อน…กลับ says "back" twice | ลอง revert fix ออก |

Don't fake sloppiness either (typos, forced slang); it reads more artificial, not less.

## Wrong sense

Pick the Thai word that fits the *meaning in context* and the *subject*. Can *this thing* actually do *that verb* in Thai?

| Bad | Source | Why | Better |
|---|---|---|---|
| ใช้ได้เองเต็มที่ | works fully on its own | เต็มที่ = "all-out", not "complete" | ใช้ได้ครบจบในตัว |
| สคริปต์พาไฟล์เข้ามา | the script brings files in | พา is for leading people/animals | ดึงไฟล์เข้ามา |
| วิ่งเทส | run the tests | วิ่ง is running on foot | รันเทส |
| ถือ error | handles errors | ถือ = hold in your hand | จัดการ error |
| ร่างนี้คือฉบับจริง | the draft becomes the final version | คือ = "is"; loses the change | ร่างนี้กลายเป็นฉบับจริง |
| ให้บริการทุกทีม | serves every team | ให้บริการ sounds like customer service | ใช้ได้กับทุกทีม |
| ค่าที่คาด | expected value | translated term nobody says | expected / ค่าที่คาดหวัง |

## English verbs/adjectives in Thai verb slots

- ข้อมูลออกไป govern แล้ว → ข้อมูลที่ส่งออกไปจึงได้มาตรฐาน
- วาง standard → วางมาตรฐาน (fixed Thai collocation)
- Coined English words are a tell too: un-normalized, de-scaled.

## Literal metaphors

| Bad | English behind it | Better |
|---|---|---|
| ตั้งพื้นของ timeout ไว้ที่ X | floor | ให้ timeout ต่ำสุดเป็น X |
| 100 คือเพดานที่ตั้งไว้ | ceiling / cap | 100 คือ limit ที่ตั้งไว้ |
| ไม่ได้ช่วยในเส้นทางนี้ | code path | ไม่ได้ช่วยในเคสนี้ |
| เส้นแบ่ง frontend/backend ถูกอยู่แล้ว | the frontend/backend line | ส่วนของ frontend กับ backend แยกกันถูกอยู่แล้ว |
| ย้ายไป comment ซึ่งเป็นที่ของมัน | where it belongs | ย้ายไปไว้ใน comment แทน (drop the phrase) |
| อยากได้ตัวชี้ไป doc | pointer to the doc | จะได้ตามไปอ่าน doc ต่อได้ |
| ให้ cache รับหน้าที่ตรงนี้ | take on the role | ใช้ cache ทำตรงนี้แทน |
| เชนที่เกิด: | the chain | มันวนแบบนี้: |
| ถาม server ใหม่ทุก 5 วินาที | re-ask (a request) | เช็ก server ใหม่ทุก 5 วินาที |
| รับสองสถานะ | handles two states | เจอได้จริงสองกรณี |
| ย่อหน้านี้ | this paragraph (`<p>`) | ข้อความนี้ |

## English structure

- **Noun-phrase UI chips** ("Settings have no history"): describe what goes wrong.
  - การตั้งค่าไม่มีประวัติ → แก้ค่าแล้วย้อนดูไม่ได้ว่าเดิมตั้งไว้เท่าไร
- **Lead with the problem, then what's missing**: `มี X เดียว ไม่แยก A กับ B`.
  - "One Delete for both archive and trash" → มีปุ่ม Delete ปุ่มเดียว ไม่แยกเก็บเข้าคลังกับลบทิ้ง
  - Topic–comment order also works: ไฟล์ที่จะเก็บกับไฟล์ที่จะทิ้ง ใช้ปุ่ม Delete ปุ่มเดียวกัน
- **Stacked negatives**: ไม่แยกว่าไม่เกี่ยว… (restructure as above).
- **Mirrored "no longer"**: "ไม่ได้…แล้ว" also reads as "and then". Name the old state: จากเดิมที่… ตอนนี้…
- **Clause order that shifts the subject**: "What the old version did well, v2 keeps" ≠ ที่ทำได้ดีแล้ว v2 เก็บไว้ (reads as v2 already does it well). → ข้อดีของเวอร์ชันเก่าที่ v2 เก็บไว้
- **Over-compression**: sync ไม่ซ้ำ ("sync doesn't repeat"?) → sync ซ้ำได้โดยข้อมูลไม่ซ้ำ
- **Literal counts/classifiers**: ไฟล์หนึ่งไฟล์ → ไฟล์หนึ่ง
- **Whole clauses in English shape**:
  - ซึ่งตรงกับเจตนาที่ประกาศค่าคงที่นั้นไว้แต่แรก ("matches the intent of declaring that constant") → ซึ่งก็คือที่ตั้งค่านี้ไว้ตั้งแต่แรก
  - ไม่แน่ใจว่าคุ้มกับความซับซ้อนที่เพิ่ม ("worth the added complexity") → ไม่แน่ใจว่าคุ้มไหม เพราะโค้ดจะซับซ้อนขึ้น
  - ข้อเสียที่มีจริงคือ… ("the real downside is") → ที่เสียจริง ๆ คือ… / แต่…
  - "ค่า limit ถูก normalize ซ้ำอีกชั้น" (vague, hides the cause) → ค่า limit ถูกหารสองรอบ

## Missing Thai words

- แอปที่ทีมทำงานทุกวัน → แอปที่ทีม**ใช้**ทำงานทุกวัน
- รู้จัก Foo กับ Bar (reads as a statement) → **มา**รู้จัก Foo กับ Bar / **ขอแนะนำ** Foo กับ Bar

## Broken mechanics

- **Doubled words**: เป็นทั้ง A และเป็นทั้ง B → เป็นทั้ง A และ B
- **Run-ons that parse wrong**: ไม่ใช่ข้อบังคับทีมที่ไม่สะดวก… (reads as "not a requirement of the teams that…") → ไม่ได้บังคับ ถ้าทีมไหนไม่สะดวก… ก็…
- **Stray spaces from stripped formatting**: ปัญหาคือ ค่า default ไม่ใช่ ค่าที่ user ตั้ง (bold removed, spaces left). Remove them, or keep the formatting.

## Translationese markers

- Extra pronouns (ฉัน/มัน in every sentence). คุณ in team chat (ข้อสรุปของคุณ) sounds stiff: drop it or use the name. คุณ addressing a customer in copy is fine.
- Filler verbs: ทำการ…, ดำเนินการ…, การทำการตรวจสอบ → just the verb: ตรวจ, แก้
- Passive ถูก: ไฟล์ที่ถูกสร้าง → ไฟล์ที่สร้างไว้
- Essay connectors: นอกจากนี้, อย่างไรก็ตาม
- Assistant voice: แน่นอน!, หวังว่าจะเป็นประโยชน์
- Em dashes (—) in every message: a space or แล้วก็ usually works. Minor.

## Over-explaining and overclaiming

- Justifying an obvious action: เพิ่ม comment ไว้แล้ว คนที่มาอ่านทีหลังจะได้ไม่ต้อง… → just say it's done.
- Dense parentheticals → split into a short plain sentence.
- Overclaiming: "same size" is not "identical every byte". Say what you checked (ขนาดไฟล์เท่ากัน), or check more.

## Inconsistency

Code-mixing defaults for tech/product teams, with examples:

- **English**: UI labels (Save, Cancel, Settings), output types (Report, Dashboard), dev nouns (sync, export, label, PR).
- **Thai**: มาตรฐาน (not standard), เครื่องมือ, ขั้นตอน, ระบบ.
- **Transliterated** where teams say it that way: โปรดักต์. Keep loanword spelling consistent.
- Unsure what the team says (หัวหน้าทีม vs ลีด, product vs โปรดักต์)? Pick one and flag it.
- **Parallel lists stay parallel**: ทีมเดียวกัน โค้ดเดียวกัน กำหนดการเดียวกัน (not …, ใช้กำหนดการเดียวกัน).
- **Word choice per register**: dev over นักพัฒนาซอฟต์แวร์ in chat; never ครับ on every sentence.

## Wordplay and allusions

- "Our App and the Chamber of Secrets" → แอปของเรากับห้องแห่งความลับ (echoes the Thai title แฮร์รี่ พอตเตอร์กับห้องแห่งความลับ)
- A metaphor that maps to a concept ("follow the recipe; the recipe is the spec") uses the same Thai word in both places: ทำตามสูตร … สูตรคือ spec
- ของจริง carries both "real" and "the real deal", like "the real thing".
- Avoid clichés that flatten the tone: จากความฝันสู่ความจริง

## Plain mode: what reads human

- Narrate how you found things: ไล่ดูแล้วเจอว่า…
- Side notes as ปล.: ปล. ข้อมูลเก่ายังไม่ได้ migrate นะ เดี๋ยวแยก PR
- Casual abbreviations where natural: กทม., ฯลฯ

## Copy mode

Reference: polished Thai product copy, e.g. Apple's Thai site (apple.com/th). Patterns seen there:

- Introductions: ขอแนะนำ X, มาทำความรู้จักกับ X, ใหม่ X. Title pattern: จาก… สู่…
- Short taglines in fragments, not full sentences: บางเบาเหลือเชื่อ
- Rhythm and rhyme: เก่งล้นตัว คุ้มเหลือล้น, เร็วดีไม่มีตก
- Elevated adjectives: เหนือชั้น, น่าทึ่ง

Don't make up rhymes or slogans that only sound clever in English logic; if a rhyme doesn't come naturally, a plain fragment is better.
