# Unity Payer Movement
<br>
Movimentação do player com teclado
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

<br>
Movimentação do player com mouse
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
        float H = Input.GetAxis("Mouse X"); // Movimento
        float V = Input.GetAxis("Mouse Y"); // Movimento
        //float H = Input.GetAxis("Mouse ScrollWheel"); // Scroll
        //float H = Input.GetAxis("Fire1"); // Clique
        //float V = Input.GetAxis("Fire2"); // Clique

        transform.Translate(new Vector3(H * Time.deltaTime * velocidade, V * Time.deltaTime * velocidade,0)); 

    }
}
```
