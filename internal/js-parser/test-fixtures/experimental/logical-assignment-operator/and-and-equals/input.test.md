# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `experimental > logical-assignment-operator > and-and-equals`

### `ast`

```javascript
JSRoot {
	body: [
		JSExpressionStatement {
			expression: JSLogicalExpression {
				operator: "&&"
				left: JSReferenceIdentifier {
					name: "a"
					loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:0-1:1 (a)
				}
				right: JSReferenceIdentifier {
					name: "INVALID_PLACEHOLDER"
					loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:4-1:5
				}
				loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:0-1:5
			}
			loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:0-1:5
		}
		JSExpressionStatement {
			expression: JSReferenceIdentifier {
				name: "b"
				loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:6-1:7 (b)
			}
			loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:6-1:8
		}
		JSExpressionStatement {
			expression: JSLogicalExpression {
				operator: "&&"
				left: JSMemberExpression {
					object: JSReferenceIdentifier {
						name: "obj"
						loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:0-2:3 (obj)
					}
					property: JSStaticMemberProperty {
						value: JSIdentifier {
							name: "a"
							loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:4-2:5 (a)
						}
						loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:4-2:5 (a)
					}
					loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:0-2:5
				}
				right: JSReferenceIdentifier {
					name: "INVALID_PLACEHOLDER"
					loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:8-2:9
				}
				loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:0-2:9
			}
			loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:0-2:9
		}
		JSExpressionStatement {
			expression: JSReferenceIdentifier {
				name: "b"
				loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:10-2:11 (b)
			}
			loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 2:10-2:12
		}
	]
	comments: []
	corrupt: true
	diagnostics: [
		{
			origins: [{entity: "ParserCore<js>"}]
			description: {advice: [], category: ["parse"], categoryValue: "js", message: [RAW_MARKUP {value: "Unknown start to an "}, "statement expression"]}
			location: {
				language: "js"
				path: UIDPath<experimental/logical-assignment-operator/and-and-equals/input.js>
				end: Position 1:4
				start: Position 1:4
			}
		}
	]
	directives: []
	hasHoistedVars: false
	sourceType: "script"
	syntax: []
	path: UIDPath<experimental/logical-assignment-operator/and-and-equals/input.js>
	loc: SourceLocation experimental/logical-assignment-operator/and-and-equals/input.js 1:0-3:0
}
```

### `diagnostics`

```

 experimental/logical-assignment-operator/and-and-equals/input.js:1:4 parse(js) ━━━━━━━━━━━━━━━━━━━━

  ✖ Unknown start to an statement expression

  > 1 │ a &&= b;
      │     ^
    2 │ obj.a &&= b;


```
