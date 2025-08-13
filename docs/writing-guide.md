## 文档撰写规范

### 总体要求
- 简明、准确、可验证。
- 每个公共符号须包含: 说明、签名、参数、返回值、示例、注意事项（如有）。

### 代码注释约定
- TypeScript/JavaScript 使用 JSDoc/TSDoc:
```ts
/**
 * 返回两个数字的和
 * @param a 第一个数字
 * @param b 第二个数字
 * @returns 两数之和
 */
export function add(a: number, b: number): number {
  return a + b;
}
```

- Python 使用 docstring（Google/Numpy 风格其一）:
```python
def add(a: int, b: int) -> int:
    """返回两个数字的和。

    Args:
        a: 第一个数字
        b: 第二个数字

    Returns:
        两数之和
    """
    return a + b
```

### 示例与可运行性
- 示例应尽量可复制运行，注明前置条件或依赖。
- 涉及外部服务时，提供最小可运行替代方案或 mock。

### 版本与兼容性
- 在发生破坏性变更时，更新示例并给出迁移指南。
- 使用 “自 x.y.z 版本起” 标注新增功能。