# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `typescript > class > duplicate-modifier-2`

### `ast`

```javascript
JSRoot {
	body: [
		JSClassDeclaration {
			id: JSBindingIdentifier {
				name: "A"
				loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 1:6-1:7 (A)
			}
			meta: JSClassHead {
				body: [
					JSClassProperty {
						key: JSStaticPropertyKey {
							value: JSIdentifier {
								name: "foo"
								loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 2:32-2:35 (foo)
							}
							loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 2:32-2:35
						}
						meta: JSClassPropertyMeta {
							abstract: false
							optional: false
							readonly: false
							static: false
							loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 2:32-2:35
							start: Position 2:32
						}
						loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 2:32-2:36
					}
				]
				loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 1:0-3:1
			}
			loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 1:0-3:1
		}
	]
	comments: []
	corrupt: false
	diagnostics: [
		{
			origins: [{entity: "ParserCore<js>"}]
			description: {
				advice: []
				category: ["parse"]
				categoryValue: "js"
				message: RAW_MARKUP {value: "Unknown class property start"}
			}
			location: {
				language: "js"
				path: UIDPath<typescript/class/duplicate-modifier-2/input.ts>
				end: Position 2:10
				start: Position 2:10
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "module"
	syntax: ["ts"]
	path: UIDPath<typescript/class/duplicate-modifier-2/input.ts>
	loc: SourceLocation typescript/class/duplicate-modifier-2/input.ts 1:0-4:0
}
```

### `diagnostics`

```

 typescript/class/duplicate-modifier-2/input.ts:2:10 parse(js) ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Unknown class property start

    1 │ class A {
  > 2 │   declare public static declare foo;
      │           ^
    3 │ }


```
