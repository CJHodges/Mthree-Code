def permute_stack(name):
    stack = [(name, "")]  # (remaining, built_so_far)
    result = []

    while stack:
        remaining, built = stack.pop()
        if not remaining:
            result.append(built)
        else:
            for i in range(len(remaining)):
                stack.append((remaining[:i] + remaining[i+1:], built + remaining[i]))
    return result

# Example
print(permute_stack("abc"))
