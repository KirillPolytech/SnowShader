# SnowShader

Шейдер снега для Unity HDRP/Shader Graph.

## Особенности

- Деформация снега на основе Render Texture.
- Совместимость с High Definition Render Pipeline (HDRP).
- Настраиваемые параметры:
<br/>MainTexture - основная текстура снега. <br/>
Metallic - металик <br/>
BaseMapTiling - тайлинг MainTexture <br/>
Bottom Color - цвет нижней части снега при деформации. <br/>
Normal Texture - текстура нормали снега. <br/>
NormalMapTiling - тайлинг NormalMap. <br/>
NormalStength - сила карты нормали. <br/>
HeightMap - карта высот (текстура) для деформации (RenderTexture). <br/>
HeightMultiplier - высота снега. <br/>
BottomHeight - переменная для определения высоты цвета при деформации. <br/>
EdgeFadeStart - в процессе. <br/>
EdgeFadeEnd - в процессе. <br/>
Splat Dissolve - переменная для размытия границ при деформации. В основном в диапазоне [0,1] <br/>
Noise Texture - текстура шума. <br/>
Noise Tiling - тайлинг для Noise Texture. <br/>
Noise Sparkling - в процессе. <br/>
Tesselation Factor - сила тесселяции. <br/>
 
## Скриншоты

![Пример снега на объекте](Screenshots/Example1.png)  
![Снег на террейне](Screenshots/example2.png)

# Предупреждения

Для корректной работы шейдера текстура кисти должна использовать Wrap Mode, отличный от Repeat, и не должна касаться своих собственных краев. Background кисти должен быть белым.

For the shader to work correctly, the brush texture must use a Wrap Mode other than Repeat, and it must not touch its own edges. The background of the brush should be white.
