# Конвертирование позиции UI элемента в мировые координаты игрового пространства
``` C#
public Vector3 GetWorldPositionFromUI(RectTransform uiElement)
{
    Camera mainCamera = Camera.main;

    // Получаем позицию UI элемента на экране
    Vector2 screenPos = RectTransformUtility.WorldToScreenPoint(null, uiElement.position);

    // Преобразуем в мировые координаты игрового пространства
    Vector3 worldPos = mainCamera.ScreenToWorldPoint(new Vector3(screenPos.x, screenPos.y, mainCamera.nearClipPlane + 5f));

    return worldPos;
}
```
