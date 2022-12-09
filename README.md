# Unity Payer Movement
<br>
Movimentação do player com teclado e mouse
<br>

```C#
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Player : MonoBehaviour
        
{

    public float velocidade = 5f;

    void Update()
    {
        float H = Input.GetAxis("Horizontal");
        float V = Input.GetAxis("Vertical");

        transform.Translate(new Vector3(H * Time.deltaTime * velocidade, V * Time.deltaTime * velocidade, 0));

    }
}
```
