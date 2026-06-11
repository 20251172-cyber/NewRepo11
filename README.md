using System;

namespace APP3C
{
    public class BebidaEnergetica : Bebida
    {
        public int NivelCafeina { get; set; }
        public bool ContieneTaurina { get; set; }

        public BebidaEnergetica(
            string nombre,
            decimal precio,
            int nivelCafeina,
            bool contieneTaurina)
            : base(nombre, precio)
        {
            NivelCafeina = nivelCafeina;
            ContieneTaurina = contieneTaurina;
        }

        public override string MostrarInformacion()
        {
            return $"Bebida Energética: {Nombre} | " +
                   $"Precio: ${Precio} | " +
                   $"Cafeína: {NivelCafeina} mg | " +
                   $"Taurina: {private void btnAgregar_Click(object sender, EventArgs e)
{
    string nombre = txtNombre.Text;
    decimal precio = decimal.Parse(txtPrecio.Text);
    int cafeina = int.Parse(txtCafeina.Text);
    bool taurina = chkTaurina.Checked;

    BebidaEnergetica bebida = new BebidaEnergetica(
        nombre,
        precio,
        cafeina,
        taurina);

    lstBebidas.Items.Add(
        bebida.MostrarInformacion());
}(ContieneTaurina ? "Sí" : "No")}";
        }
    }
}


