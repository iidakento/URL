# URL
オブジェクトに触れると紹介サイトへ移動するかのメッセージの表示
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class URL : MonoBehaviour
{
    //オブジェクトが衝突した時
    void OnCollisionEnter(Collision collision)
    {
        bool isOK = UnityEditor.EditorUtility.DisplayDialog("メッセージ","紹介サイトへ移動します", "OK","cancel");
        if(isOK)
        {
            Application.OpenURL("http://google.co.jp/");
        }else
        {

        }
        
    }
}
