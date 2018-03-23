# STM32_API

## HAL_GPIO

> Initializes the GPIOx peripheral according to the specified parameters in the GPIO_Init.
void HAL_GPIO_Init(GPIO_TypeDef  *GPIOx, GPIO_InitTypeDef *GPIO_Init)

```C
void HAL_GPIO_DeInit(GPIO_TypeDef  *GPIOx, uint32_t GPIO_Pin);
```

> De-initializes the GPIOx peripheral registers to their default reset values.

```C
void HAL_GPIO_DeInit(GPIO_TypeDef  *GPIOx, uint32_t GPIO_Pin);
```

> Reads the specified input port pin. Return the input port pin value.

```C
GPIO_PinState HAL_GPIO_ReadPin(GPIO_TypeDef* GPIOx, uint16_t GPIO_Pin);
```

> Sets or clears the selected data port bit.

```C
void HAL_GPIO_WritePin(GPIO_TypeDef* GPIOx, uint16_t GPIO_Pin, GPIO_PinState PinState);
```

> Toggles the specified GPIO pins.

```C
void HAL_GPIO_TogglePin(GPIO_TypeDef* GPIOx, uint16_t GPIO_Pin);
```

> Locks GPIO Pins configuration registers. Return HAL_OK / HAL_ERROR.

```C
HAL_StatusTypeDef HAL_GPIO_LockPin(GPIO_TypeDef* GPIOx, uint16_t GPIO_Pin);
```

> This function handles EXTI interrupt request.

```C
void HAL_GPIO_EXTI_IRQHandler(uint16_t GPIO_Pin);
```

> EXTI line detection callbacks.

```C
__weak void HAL_GPIO_EXTI_Callback(uint16_t GPIO_Pin);
```